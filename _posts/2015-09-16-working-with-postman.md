---
title: 'Working with Postman'

layout: nil
---


This will serve a guide on how to setup Postman to successfuly test/execute the MSG web services/api. 
Postman is a Web REST client that allows you to enter and monitor HTTP requests and responses.
This guide uses Postman Google Chrome Extension

###Steps:

###1. Under "Authorization" tab, select "Basic Auth" in the dropdown list. 
<div style="border: 1px solid #bfbfbf; margin-bottom: 50px;">
    <img src="images/using_postman_auth.png" alt="using_postman_auth">
</div>

###2. Input the Username and Password credentials (provided by the Administrator/Super User). Then click the "Update request" button.
```Username: msg
Password: passwordmsg
```
<div style="border: 1px solid #bfbfbf; margin-bottom: 50px;">
    <img src="images/using_postman_auth_input.png" alt="using_postman_auth_input">
</div>

###3. Select "POST" in the dropdown list located above the tabs. 
```Method: POST```
<div style="border: 1px solid #bfbfbf; margin-bottom: 50px;">
    <img src="images/using_postman_dropdown_request.png" alt="using_postman_dropdown_request">
</div>

###4. Input the request URL path.
```http://msg.rpdata.com/ttsvr/msg?```
<div style="border: 1px solid #bfbfbf; margin-bottom: 50px;">
    <img src="images/using_postman_url_request_path.png" alt="using_postman_url_request_path">
</div>

###5. Under the "Body" tab, choose "raw". Then select "JSON(application/json)" in the dropdown list.
```Request Body: raw
Data Type: JSON(application/json)```
<div style="border: 1px solid #bfbfbf; margin-bottom: 50px;">
    <img src="images/using_postman_body.png" alt="using_postman_body">
</div>



###Note:
After Step 5, the "Headers" tab should be automaticaly updated with the following sample;
```Authorization: Basic bXNnOkU3bVc6JTZ7REs=
Content-Type: application/json```
<div style="border: 1px solid #bfbfbf; margin-bottom: 50px;">
    <img src="images/using_postman_headers_input.png" alt="using_postman_headers_input">
</div>


The input box under the "Boby" tab is where you place the request parameters. 
See sample below;
```{
    "op": "getMobilePropertyAdditionalInfo",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "propertyId": "7764519"
}```
<div style="border: 1px solid #bfbfbf; margin-bottom: 50px;">
    <img src="images/using_postman_body_paramaters.png" alt="using_postman_body_paramaters">
</div>
