
# React GitHub Lik Graph Component


This React component provides a visual representation similar to the GitHub contribution graph, displaying daily work statuses using colored boxes. Users can pass a dataset containing date and work type information to render the graph.

## Installation

Install ReactGithubLikeGraph with npm

```bash
  npm install react-github-like-graph

```
    
## Usage

Import the component and use it within your React application:
```bash
import React from 'react';
import ReactGithubLikeGraph from 'react-github-like-graph';
import 'react-github-like-graph/App.css'; // Include the CSS file if needed

const YourComponent = () => {
  
  const dataset = [
    { date: 1412225727246, type: 'hard' },
    { date: 1512225727247, type: 'medium' },
    { date: 1612225727248, type: 'less' },
    { date: 1712225727249, type: 'none' },
    { date: 1712125727250, type: 'hard' },
    { date: 1712225727251, type: 'medium' },
    { date: 1312225727252, type: 'less' },
    { date: 1212225727253, type: 'upper-medium' }
  ];

  return (
    <div>
      <ReactGithubLikeGraph dataset={dataset} />
    </div>
  );
}

export default YourComponent;

```
## Sample Data

let data = [
    { date: 1412225727246, type: 'hard' },
    { date: 1512225727247, type: 'medium' },
    { date: 1612225727248, type: 'less' },
    { date: 1712225727249, type: 'none' },
    { date: 1712125727250, type: 'hard' },
    { date: 1712225727251, type: 'medium' },
    { date: 1312225727252, type: 'less' },
    { date: 1212225727253, type: 'upper-medium' }
  ]

### Guidance 

In the given data one object means one day , the first key should be (date) with the value which is time in miliseconds , and the another key is type which means the color ,now below i have written the types with color codes, 

##### none = #ebedf0
##### less = #9be9a8
##### medium = #40c463"
##### upper-medium = #30a14e
##### hard = #216e39