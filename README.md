# run-time-polymorphism

class people{
    void profession(){
        System.out.println("people have profession");
    }
}
class doctor extends people{
    void profession(){
        System.out.println("doctors cures patients");
    }
}
class teacher extends people{
    void profession(){
        System.out.println("teachers teaches class");
    }
}
class plumber extends people{
    void profession(){
        System.out.println("plumber fixes pipe");
    }
}
class engineer extends people{
    void profession(){
        System.out.println("engineer builds house");
    }
}


public class RunTime {

    public static void main(String[] args) {
        people myDoctor = new doctor();
        people myTeacher = new teacher();
        people myPlumber = new plumber();
        people myEngineer = new engineer();
        
        myDoctor.profession(); 
        myTeacher.profession(); 
        myPlumber.profession(); 
        myEngineer.profession(); 
    }
}
        
        
run:


doctors cures patients
teachers teaches class
plumber fixes pipe
engineer builds house
