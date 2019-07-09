# Google I/O 2019 Extended Radzymin - live coding
 Angular + Nest + Firebase web app developed during Google I/O 2019 Extended Radzymin.
 
 
 ### How to run this:
 You need to have NodeJS installed.
 1) clone or download this repository
 2) go to the project folder
 
 
 ### Backend:
 3) go to "io19ext-backend" folder and open it using your favorite IDE (VS Code)
 4) run command: npm install
 5) run command: npm start
 6) open a web browser and go to: localhost:3000
 7) you should see "Hello World!" message
 
 
 ### Frontend:
 8) go to "io19ext" folder and open it using your IDE
 9) run command: npm install
 10) go to src/app/events/containers and open events.component.ts
 11) uncomment this.events$ = this.eventsService.getEventsFromBackend(); line and comment firebase line
 12) run command: ng serve
 13) test it in your browser (you need to have backend server running), type: localhost:4200
 14) you should see the list of cards 

 ### Note for Firebase:
 - you need to create an account and a project with Firestore database
 - put your Firebase project settings into: src/environments/firebase.config.ts
 - you need to add some data to the Firestore database:
  - add "Events" collection
  - add some items there, something like this:
  
    {
    
        name: 'Google I/O 19 Ext Radzymin',
        description: 'To jest opis eventu',
        photoUrl: 'https://secure.meetupstatic.com/photos/event/e/9/c/b/highres_480839851.jpeg'
     },
     {
     
        name: 'GDG Radzymin #7',
        description: '7 event GDG Radzymin',
        photoUrl: 'https://secure.meetupstatic.com/photos/event/c/a/9/a/highres_478491866.jpeg'
      },
      {
      
        name: 'DevFest Radzymin',
        description: 'DevFest Radzymin w 2018',
        photoUrl: 'https://secure.meetupstatic.com/photos/event/e/4/2/5/highres_475438405.jpeg'
      }
      
If you have any problems try to restart your computer and if it won't help you can ask me 😂
