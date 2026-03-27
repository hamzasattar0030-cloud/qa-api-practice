# Postman API Test Case

## TC001 - Verify valid post endpoint returns correct response

**Tool:** Postman  
**Method:** GET  
**Endpoint:** /posts/1  

### Steps
1. Open Postman
2. Create a GET request to:
   `https://jsonplaceholder.typicode.com/posts/1`
3. Click **Send**

### Expected Result
- Status code is 200
- Response contains `id = 1`
- Response contains a non-empty `title`

### Test Script
```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response contains correct post ID", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData.id).to.eql(1);
});

pm.test("Response contains a title", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData.title).to.not.be.empty;
});

## TC002 - Verify invalid post endpoint returns empty response

**Tool:** Postman  
**Method:** GET  
**Endpoint:** /posts/9999  

### Steps
1. Open Postman
2. Create a GET request to:
   `https://jsonplaceholder.typicode.com/posts/9999`
3. Click **Send**

### Expected Result
- Status code is 404 OR response is empty (`{}`)

### Test Script
```javascript
pm.test("Status code is 404 or empty response", function () {
    pm.expect(
        pm.response.code === 404 || pm.response.text() === "{}"
    ).to.be.true;
});
