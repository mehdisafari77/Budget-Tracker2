# Budget-Tracker2
A budget tracker that can be used as a progressive web app (PWA)

## Deployed Link
https://budget-tracker2-mehdi.herokuapp.com/

## Summary
This is a budget tracking app, you can add money, or substract money from your virtual account, and track the data in your dashboard. This is a progressive web app that can be downloaded on your phone and used. 

## Screenshot Of Main Screen
<img width="1237" alt="Screenshot 2021-11-17 at 15 46 43" src="https://user-images.githubusercontent.com/75599021/142302236-d79ba088-8b3f-4b47-bf63-217122ee8c87.png">

## Built With
* [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* [Node.js](https://nodejs.org/en/docs/)
* [NPM-Library](https://docs.npmjs.com/)
* [Expres.js](https://expressjs.com/)
* [Sequelize](https://sequelize.org/master/index.html)
* [mongodb](https://www.mongodb.com/)

## Installation Steps For Local Running
1. Clone project.
2. Open terminal and run these commands in order
    - npm install
    - npm start

## Code Snippet Adding Transaction
```javascript
router.post("/api/transaction", ({ body }, res) => {
  Transaction.create(body)
    .then(dbTransaction => {
      res.json(dbTransaction);
    })
    .catch(err => {
      res.status(400).json(err);
    });
});

```

## Author

* **Mehdi Safari**

- [Link to Portfolio Site](https://mehdisafari77.github.io/Basic-Bio/)
- [Link to Github](https://github.com/mehdisafari77)
- [Link to LinkedIn](https://www.linkedin.com/in/mehdi-safari-992799142/)
