# Clock
Clock made with Basic HTML CSS JS

![5ddall](https://user-images.githubusercontent.com/70858211/122096255-fe485180-ce2b-11eb-9671-b655b55ef4cd.gif)

---
Javascript Code

```javascript
     const hourHand = document.querySelector('[data-hour-hand]')
      const minuteHand = document.querySelector('[data-minute-hand]')
      const secondHand = document.querySelector('[data-second-hand]')

      const time = () => {
        const current_date = new Date();
        const second = current_date.getSeconds() / 60;
        const minutes = (second + current_date.getMinutes()) / 60;
        const hours = (minutes + current_date.getHours()) / 12

	      setTime(secondHand,second)
	      setTime(minuteHand,minutes)
	      setTime(hourHand,hours);
    }

    const setTime = (element, rotationRatio) => {
   	element.style.setProperty('--rotation', rotationRatio * 360)
  }

setInterval(time, 1000);

time();
```

---

Links

[Visit Here](https://yogeshrdr.github.io/Clock/)
