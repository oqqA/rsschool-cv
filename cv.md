# Igor Statenin

### Contacts
* Telegram: [@oqqax](https://t.me/oqqax)
* Mail: oqqa.vw@gmail.com
  
### Summary
I am universal developer. Developed backend and android applications at freelance. I've been sick all past year and now I want to get back into development. And now I need frontend skills for my projects.

### Skills
Programming Languages: C#, C++, Python, Kotlin, JS, SQL
Frontend stack: Angular, HTML, CSS/SASS, Figma
Backend stack: ASP.NET Core, NodeJS, Express, Koa
Android stack: Jetpack Compose, Room, Koin, Coroutines, Clean + mvvm
Tools: Git, Unix/Linux, Docker, PostgreSQL, CI/CD

### Code expample
```js
// formatDuration(3662)
// => "1 hour, 1 minute and 2 seconds"

function formatDuration (seconds) {
    if (seconds === 0) return 'now';

    const durations = { 
      second: 60, 
      minute: 60*60, 
      hour:   60*60*24, 
      day:    60*60*24*365, 
      year:   60*60*24*365*100
    }
    
    let result = []
    let last_value = 1
    
    Object.entries(durations).forEach(([key,value]) => {
      
        let count = Math.floor( seconds % value / last_value )
        last_value = value
        
        if (count > 0) {
          result.unshift(count + " " + key + (count > 1 ? "s" : "") )
        }
    })
  
    return result.join(", ").replace(/,([^,]*)$/,' and'+'$1')
}
```
### Edication

* Code-basics (Hexlet)
* RS School (in proccess)

### Language
* Russian - naive
* English - B1