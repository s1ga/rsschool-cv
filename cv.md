# Sergey Harlanov

## Contact information
**Phone:** +375 (29) 122-12-68  
**Email:** s.v.harlanov@gmail.com  
**Discord:** s1ga
- - -

## Summary
- - -

## Skills
**Languages:** HTML, CSS, JS, SQL  
**Frameworks:** React, Node.js, Express.js,   
**Technologies:** GIT, Docker, Swagger, Redux, Saga  
**Software:** Webstorm, Visual Studio Code, Figma 

- - -

## Code example
~~~
// Self implementation of event emitter 
export class Emitter {
    constructor() {
        this.listeners = {}
    }

    emit(event, ...args) {
        if (!Array.isArray(this.listeners[event])) {
            return false
        }
        this.listeners[event].forEach(listener => {
            listener(...args)
        })

        return true
    }

    subscribe(event, fn) {
        this.listeners[event] = this.listeners[event] || []
        this.listeners[event].push(fn)
    
        return () => {
            this.listeners[event] = this.listeners[event].filter(listener => listener !== fn)
        }
    }
}
~~~
- - -

## Education
### Belarusian State University (2019 - present)  
Mechanics and Mathematics faculty, Bachelor

- - -

## English 
**Level:** A2 - B1
