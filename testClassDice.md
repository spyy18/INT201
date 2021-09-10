ทดลองสร้าง Dice Game แบบใช้ class

```javaScript
class Dice {

    constructor(gameTitle) { //รับ parameter gameTitle คือชื่อเกมที่ใช้ลูกเต๋ษนี้ในการเล่น
    
      this._diceName = (gameTitle===undefined ? "Unknow" : gameTitle); 
      /*this._diceName คือ attribute  ที่มีการกำหนดให้มีค่าเป็น ค่าที่ได้จากเงื่อนไข if 
      ถ้า parameter gameTitle ไม่ได้รับค่าอะไรมาเลย ให้ this._diceName มีค่าเป็น Unknown
      ถ้ารับมาก็ให้ this._diceName มีค่าเป็นค่านั้น*/
      
      this._faceValue = Math.floor(Math.random() * 6) + 1; 
      /*this._faceValue คือ attribute  ที่มีการกำหนดให้มีค่าเป็น ค่าที่ได้จากการสุ่มตัวเลข*/
    }

    get faceValue(){
        console.log("Getter is Working");
        return this._faceValue;
    }
    //ถ้าใน class มีการกำหนด get เอาไว้ แล้วเรามีการเรียกใช้ตัวนั้น มันจะเข้ามาทำสิ่งที่เขียนไว้ใน get 
    
    
    set faceValue(faceValue){
        console.log("Setter is Working");
        return this._faceValue;
    }
     /*ถ้าใน class มีการกำหนด set เอาไว้ แล้วเรามีเปลี่ยนแปลงค่าของตัวนั้น มันจะเข้ามาทำสิ่งที่เขียนไว้ใน set
     แต่ถ้าไม่ได้เขียน set ไว้ ตัวนั้นก็จะกลายเป็นค่าที่เราเปลี่ยนแปลง*/

    toString(){
        return `Game : ${this._diceName} , FaceValue : ${this._faceValue}`;
        //toString เป็นเหมือน รูปแบบของการแสดงผลว่าเราอยากให้มันมีหน้าตาเป็นแบบไหน ต้องเขียนเอง
    }

}
  
  
  console.log("--------------------------");
  let dice1 = new Dice();
  console.log(dice1.toString());
  //เมื่อไม่ได้ส่ง parameter ใดๆเข้าไปใน class Dice
  
  console.log("--------------------------");
  dice1["faceValue"]=5;
  //เมื่อเปลี่ยนแปลงค่า faceValue ถ้าเราเขียน set ไว้ มันจะเข้าไปทำสิ่งที่อยู่ใน set
  
  console.log("--------------------------");
  let dice2 = new Dice("Hi-lo");
  console.log(dice2.toString());
  //เมื่อส่ง parameter เข้าไปใน class Dice 


```
