หา zodiact จากปีเกิด หารด้วย 12 
```javascript
  function findZodiact(year){
    switch(year%12){
      case 0 : console.log("monkey"); 
                break;
      case 1 : console.log("rooster");
                break;
      case 2 : console.log("dog");
                break;
      case 3 : console.log("pig");
                break;
      case 4 : console.log("rat");
                break;
      case 5 : console.log("ox");
                break;
      case 6 : console.log("tiger");
                break;
      case 7 : console.log("rabbit");
                break;
      case 8 : console.log("dragon");
                break;
      case 9 : console.log("snake");
                break;
      case 10 : console.log("horse");
                break;
      case 11 : console.log("sheep");
                break;
    }
}

findZodiact(2001); //snake

```
