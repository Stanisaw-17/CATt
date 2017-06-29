# CATt
Homework1
public class Main {
    public static void main(String[] args) {
        Cat cat1 = new Cat();
        Cat cat2 = new Cat("Vasia", "white", 5, 2);
        cat1.setName("Tima");
        cat1.setColor("black");
        cat1.setWeight(10);
        cat1.setYear(8);

        System.out.println(cat1);
        System.out.println(cat2);
        cat2.voice();
        cat1.run();
    }
}
public class Cat {
    private String name;
    private String color;
    private int year;
    private double weight;
    private String gender = "male";

    public Cat(String name, String color, int year, double weight) {
        super();
        this.name = name;
        this.color = color;
        this.year = year;
        this.weight = weight;
    }

    public Cat (){
        super();
    }

    public void voice () {
        System.out.println("I can say Miay");
    }
    private String sex (String gender){
        this.gender = gender;
        return "male";}

        public void run (){
            System.out.println("i cant running because my weight " + weight);
        }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getColor() {
        return color;
    }

    public void setColor(String color) {
        this.color = color;
    }

    public int getYear() {
        return year;
    }

    public void setYear(int year) {
        this.year = year;
    }

    public double getWeight() {
        return weight;
    }

    public void setWeight(double weight) {
        this.weight = weight;
    }

    public String getGender() {
        return gender;
    }

    @Override
    public String toString() {
        return "Cat{" +
                "name='" + name + '\'' +
                ", color='" + color + '\'' +
                ", year=" + year +
                ", weight=" + weight +
                ", gender='" + gender + '\'' +
                '}';
    }
}
