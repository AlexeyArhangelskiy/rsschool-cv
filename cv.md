# Aleksei Arkhangelskii

## Contact
Berlin, Germany
arhmost@gmail.com
linkedin.com/in/aleksei-arkhangelskii
telegram @arhalexey

## Summary
Junior Fullstack Developer currently studying at 42 Berlin and RS school. I have 10 years of experience in the construction industry with a focus on BIM and design process automation. I have experience managing and collaborating with cross-functional teams and ensuring project success. I have experience writing C# plugins to automate design processes and developing internal product.

## Skills
* HTML
* CSS/Sass/Scss
* JavaScript
* C/C#
* Git

## Code Examples
```javascript
     const deadLine = '2023-01-01';

        function getTimeRemaining(endtime) {
            let days, hours, minutes, seconds;
            const t = Date.parse(endtime) - Date.parse(new Date());

            if (t <= 0) {
                days = 0;
                hours = 0;
                minutes = 0;
                seconds = 0;
            } else {
                days = Math.floor(t / (1000 * 60 * 60 * 24)),
                  hours = Math.floor((t / (1000 * 60 * 60) % 24)),
                  minutes = Math.floor((t / 1000 / 60) % 60),
                  seconds = Math.floor((t / 1000 ) % 60);
            }
                     

            return {
                'total': t,
                'days': days,
                'hours': hours,
                'minutes': minutes,
                'seconds': seconds
            };
        }

        function getZero(num) {
            if (num >= 0 && num < 10) {
                return `0${num}`;
            } else {
                return num;
            }

        }

        function setClock(selector, endtime) {
            const timer = document.querySelector(selector),
                  days = timer.querySelector('#days'),
                  hours = timer.querySelector('#hours'),
                  minutes = timer.querySelector('#minutes'),
                  seconds = timer.querySelector('#seconds'),
                  timeInterval = setInterval(updateClock, 1000);

            updateClock();      
        
            function updateClock() {
                const t = getTimeRemaining(endtime);

                days.innerHTML = getZero(t.days);
                hours.innerHTML = getZero(t.hours);
                minutes.innerHTML = getZero(t.minutes);
                seconds.innerHTML = getZero(t.seconds);

                if (t.total <= 0) {
                    clearInterval(timeInterval);
                }
            }
        }

        setClock('.timer', deadLine);
```

## Experience
2022 - Present BIM Software Engineer
2020 - 2022 Project Engineer
2013 - 2020 Structural Engineer

## Education

Ural State University of Railway Transport
Engineer's degree, Engineer Bridges and Tunnels
Sep 2010 - Jul 2015

42 Berlin
Aug 2023 - Present
Software developer in the C program language

## Language

English - B2
German - A1