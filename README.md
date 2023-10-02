# JavaProgramming



### How to Make a Dynamic Array in java inside Class
```java


// Question 2.

class CGPA {
    // int marks[] = new int[] { 0, 0, 0, 0, 0, 0, 0, 0 };
    int marks[] = new int[20]; // settting the maximum length
    int subjects;

    CGPA(int sub) {
        this.subjects = sub;
        Scanner sc = new Scanner(System.in);
        for (int i = 0; i < subjects; i++) {

            System.out.println("Enter your " + (i + 1) + " number");
            marks[i] = sc.nextInt();

        }
        sc.close();
    }

    void calculate() {
        float totalNumber = 0;
        for (int i = 0; i < subjects; i++) {
            totalNumber += marks[i];

        }
        totalNumber = (totalNumber / subjects) / 10;
        System.out.println("CGPA : " + totalNumber);

    }

    public void output() {
        for (int i = 0; i < subjects; i++) {
            System.out.print(marks[i] + " ");

        }
    }
}


```


## Ternary Operator in java

### Ternary Operator in java returns come value so it should be assigned to some vlaue like i did above

```java

class GreaterOrNot {
    int given;
    int userinput;

    GreaterOrNot(int given) {
        this.given = given;
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number");
        this.userinput = sc.nextInt();
        String value = given > userinput ? "given greater than userinput"
                : "Userinput is greater than given";

        System.out.println(value);

        sc.close();

    }

}

```




