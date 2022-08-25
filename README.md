<img src="./assets/Screenshot 2022-06-29 100133.jpg" />

<br/>

---

<br />

## List of Contents
1. [Introduction and demo](#mindactivity-app-for-managing-stress)
2. [Features](#features)
3. [Getting Started](#getting-started)
4. [Tech Stack](#tech-stack)
5. [Running Tests](#running-tests)
6. [Authors](#authors)
7. [Appendix](#appendix)

<br/>

---

<br />

# ***Mindactivity App For Managing Stress🧘***

Welcome to Mindactivity!


Mindactivity (Mindfulness + Activity) is a meditative media app which allows users to time their meditation and deep work sessions. Here's a little demo of the app:


https://user-images.githubusercontent.com/101634716/186674458-62721b43-b845-42d6-8f6b-a83c6a662e37.mp4


<br/>

*This documentation is for the entire Mindactivity app. If you're interested in the backend/API specifically, go to [my fork of the backend repository](https://github.com/AureaFlamma/Mindactivity_backend.git)*

<br/>

*This is a fork of the Mindactivity frontend repo. Original repos can be found here: [frontend](https://github.com/SchoolOfCode/w9_frontend-project-mindactivity.git) & [backend](https://github.com/SchoolOfCode/w9_backend-project-mindactivity). All links from this point onward point to the original repos.*




<br/>

---

<br />


## ***Features🎩***
- Timer for meditation or exercise.
- Music button playing calming nature sounds.
- Daily affirmations randomised and displayed from database.
- Blog posts also randomised and displayed from database.
- Click- and hover-interactive background simulating a night sky.

<br/>

---

<br />

## ***Getting Started🏁***


### **Backend** ###

**It is important to get the backend working before you run the frontend in order to use the affirmations and the blog post features*
1. Fork the original backend repository. You can find it [here](https://github.com/SchoolOfCode/w9_backend-project-mindactivity).
2. Clone the forked repo to your computer. Unless you renamed the repo whilst forking, the command is (insert your GitHub username where indicated): 
```bash
  git clone https://github.com/<YOUR_GITHUB_USERNAME>/w9_backend-project-mindactivity
```
3. Install all the dependencies:
```bash
  npm i
```
3. Copy your database (e.g. Heroku) URL into the .env file, following the format:
```bash
 DATABASE_URL = <Database URL goes here>
```
4. Create the affirmations table in your database by running this script in the terminal:
```bash
npm run db:createAffirmationsTable
```
5. Populate the affrimations table you have just created with data from "/lib/affirmationData.js" by running this script in the terminal:
```
npm run db:populateAffirmationsTable
```
6. Now, repeat the last 2 steps for blog table. First create it...:
```bash
npm run db:createBlogTable
```
7. ...then populate it with data from "/lib/blogs.js":
```bash
db:populateBlogTable
```
8. Finally, run the server:
```bash
  npm run dev
```

### **Frontend** ###

1. For the original frontend repo. You can find it [here](https://github.com/SchoolOfCode/w9_backend-project-mindactivity)
2. Unless you have renamed the repo when you forked it, you can clone it with this command (insert your GitHub username where indicated)
```bash
  git clone https://github.com/<YOUR_GITHUB_USERNAME>/w9_backend-project-mindactivity
```
3. Install the dependencies by running this command in the terminal.  
```bash
  npm i
```
4. Navigate to this folder: *w9_frontend-project-mindactivity/Mindactivity*

5. Start the app.
```bash
  npm start
```

<br/>

---

<br />

<a name="tech-stack"/>

## ***Tech Stack⚙️***

**Client:** React, CSS, Howler, React-tsparticles
</br>
**Server:** Node, Express, PostreSQL
</br>
**Client-side Testing:** React Testing Library
</br>
**Server-side Testing:** Supertest, Jest

<br/>

---

<br />


## ***Running Tests🃏***
To run tests, run the following command
```bash
  npm test
```
<br/>

---

<br />

## ***Authors📚***

We are four bootcampers at [The School Of Code](https://github.com/SchoolOfCode) who teamed up to build an app to help solve bootcamper burnout problem for our mid-course project.

- [@AureaFlamma](https://www.github.com/AureaFlamma)
- [@EdMark11](https://www.github.com/EdMark11)
- [@anastasia-starostina](https://www.github.com/anastasia-starostina)
- [@Sadie109](https://www.github.com/Sadie109)

<br/>

---

<br />


## ***Appendix📝***
</br>

- [React](https://reactjs.org/docs/getting-started.html)
- [TSParticles Package](https://www.npmjs.com/package/express-generator-esmodules)
- [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/)
- [Howler](https://www.npmjs.com/package/howler)
