# <img src="https://media-exp1.licdn.com/dms/image/C560BAQFFB5MAXrtEiQ/company-logo_200_200/0/1659437242707?e=1669248000&v=beta&t=t4-wDGSdhVcLz_6iELwGf3eCpJIh-c8SBVG4CRLGxJE" alt="alt text" width="50" height="50">                  Xabit Technical Assessment Question and Answer


## Your React application is rendering a page very slowly. How are you going to investigate and/or fix the issue



I would start by identifying the root cause of the issue. It may be caused by adding too many components into a single bundle file, the loading of that bundle file might take more time. Another reason for slow rendering is caused due to Analytics tracking libraries, excessive CSS animations,non-optimized images, iframes, and many more. I had faced this issue before. I solved it using useMemo hooks. It helps to memorize the value between renders and helps to prevent re-rendering on React function components. To solve this kind of problem my first prospect is research. We need to structure our components in an optimized way. Using tools like react developer tools and Chrome DevTools Performance helps to debug these issues. 






## What is the difference between filter and map?

### Filter

A filter is a process of looping through an array and including or excluding elements inside that array based on a condition that is provided.
For example
const names = ['James', 'John', 'Paul', 'Rina', 'Geo'];
function App() {
 return ( <div> 
{names.filter(name => name.includes('J')).map(filteredName => ( <li> {filteredName} </li> ))}
 </div> ); 
}

`Result: James, John`

Here, using filter only the people name which includes j is displayed.

 ### Map
 
The map function is used to iterate over an array and manipulate or change data items. 
const names = ['James', 'John', 'Paul', 'Rina', 'Geo'];
function App() {
 return ( <div> 
{names.map(peopleName => ( <li> {peopleName } </li> ))}
 </div> ); 
}

`Result: James, John, Paul, Rina, Geo`

Here, using the map method all data are iterated and displayed.


## 3. What technical aspects of React do you struggle with?



I realized that it is not sufficient to learn the react only as it is just a UI library
 which is rarely enough and is never sufficient when the application grows complex. Using
 React JS alone for that purpose will only result in a bloated codebase that will become 
 hard to manage.
 
 
 I had to struggle to learn reactjs and redux at the same time. I didn't have a strong foundation
 in reactjs and I jumped into  Redux. It introduces new concepts like actions, dispatch, reducers,
and store, which makes it more complicated.


Wasted renders are one of the most common React JS problems I have faced which caused slow down the performance.
While working in a team, We need to choose a single version of react component. If any member  contrast that with web components, for instance, there may be version conflicts.
