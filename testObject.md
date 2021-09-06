โจทย์ : สร้าง object ที่มี value เป็น function อย่างน้อย 1 function
```javascript
let salaryInWork = { name:"Supichaya" , salaryPerMonth:5000 , totalMonth:5 , 
                     sumSalary:function(){ return this.salaryPerMonth*this.totalMonth}  

/*object salaryInwork เก็บข้อมูลเงินเดือนของพนักงาน
key name เก็บค่าชื่อพนักงาน
key salaryPerMonth มี value เป็นเงินเดือนที่ได้ต่อเดือน
key totalMonth มี value เป็นจำนวนเดือนที่ทำงาน
key sumSalary  มี value เป็น function การคำนวณเงินเดือนทั้งหมดที่ได้ตั้งแต่เริ่มทำงาน
*/
```

โจทย์ : สร้าง object ที่มี value เป็น Array อย่างน้อย 1 array
```javascript
let orderDetail = { order:{
                    product:"candy" ,
                    price:5 ,
                    number:5} ,
                    orderDate:"3/09/2021" ,
                    payment:"mobile banking" 
                  };
                  
/*object orderDetail เก็บข้อมูลรายการสั่งซื้อสินค้า
key order มี value เป็น object เก็บชื่อสินค้า ราคาสินค้าต่ออัน และจำนวนสินค้าที่ซื้อ
key orderDate มี value เป็นวันที่สั่งซื้อสินค้า
key payment มี value เป็นช่องทางที่ใช้ในการชำระเงิน
*/               
```

โจทย์ : สร้าง object ที่มี value เป็น Array อย่างน้อย 1 array
```javascript
let song = {artist:"T_047",
            songList:[ "Si-Khong-Fa" , "Siang-Thale" , "Magig-Hour"]
           };
                  
/*object song เก็บข้อมูลเพลงขิงศิลปินแต่ละคน
key artist มี value เป็นชื่อของศิลปิน
key songList มี value เป็น array เก็บชื่อเพลงที่แต่งโดยศิลปิน T_047
*/               
```
