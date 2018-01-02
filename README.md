# Boilerplate React app with Express server and Docker 
React ready to start developing, build ready for production. Checkout the different branches in order to find different coding styles for the main react app.

TODO:
 - [x] Add express server and build ready
 - [x] Add dockerimage
 - [ ] Add different initial react styles.
 - [ ] Documentation.
 - [ ] Expand the README.md
 - [x] Dockerfile to use yarn instead of NPM.
 - [ ] Build the testing suite ready.
 - [ ] Add branch with express ssh.
 - [ ] Add branch with optimization.
 - [ ] Add webpack.


### React
create-react-app v.1.4.0
react-router-dom v.4

### Express


### Docker
For building the docker image we have used NPM, even though we use yarn for everything else. 

Build the image with
```bash
docker build -t react-app .
```

and then run the cotainer
```bash
docker run -d -p 80:9000 --name react-app routed-react
```


***


## Branches

```bash
git checkout serve 
```
This branch serves the react app with serve instead of express.js


***


## React styling

This branch captures all the urls in a folder instead of having them around.

```bash
git checkout routes-folder 
```


This branch separates containerization of components from it's smallest units. For example you will define a form as a container of many inputs. Form will though just handle the whole state while inputs will define style and props.

```bash
git checkout container-presentational 
```
You can read more in [container components](https://medium.com/@learnreact/container-components-c0e67432e005) and [smart and dumb components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0).


```bash
git checkout react-backend-redux
```
This branch includes a redux store and a very minimal api client to connect direclty to a backend.


***


## Resources
[Speed up express] (https://expressjs.com/en/advanced/best-practice-performance.html)
[Learn about webpack](https://webpack.academy/p/the-core-concepts)  (no affiliation)
[Awesome React Components](https://github.com/brillout/awesome-react-components)
[Redux providers](https://medium.com/@timbur/react-automatic-redux-providers-and-replicators-c4e35a39f1)
[What's redux actions and reducers](https://medium.com/@timbur/provide-redux-actions-and-reducers-to-react-components-automatically-1edc257eed11)




Pull requests are welcome.