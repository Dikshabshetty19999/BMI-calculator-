# BMI-calculator-
//A JavaScript code for BMI calculation using objects and methods. This code can be modified for more than two people.
var john={
    name : 'john smith',
    mass : 65,
    height : 1.7,
    calcBmi : function(){
        this.bmi = this.mass/(this.height*this.height);
    } 
};

var mark={
    name : 'mark johnson',
    mass : 80,
    height : 1.75,
     calcBmi : function(){
        this.bmi = this.mass/(this.height*this.height);
     }
};

john.calcBmi();
mark.calcBmi();

if (john.bmi> mark.bmi) {
    console.log('john smith has higher bmi with a bmi value of ' + (john.bmi));
}
else if (john.bmi< mark.bmi) {
    console.log('mark johnson has higher bmi with a bmi value of ' + (mark.bmi));
}
else if (john.bmi === mark.bmi) {
    console.log('both have the same bmiwith the value of ' + (john.bmi));
}
