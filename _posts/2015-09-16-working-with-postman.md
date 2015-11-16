---
title: 'Working with Postman'

layout: nil
---


This will serve a guide on how to setup Postman to successfuly test/execute the MSG web services/api. 
Postman is a Web REST client that allows you to enter and monitor HTTP requests and responses.
This guide uses Postman Google Chrome Extension

###Steps:

###1. Under "Authorization" tab, select "Basic Auth" in the dropdown list. 
<table>
    <tbody>
        <tr>
        <td><img src="images/using_postman_auth.png" alt="using_postman_auth"></td>      
        </tr>
    </tbody>
</table>

###2. Input the Username and Password credentials (provided by the Administrator/Super User). Then click the "Update request" button.
```Username: msg
Password: passwordmsg
```

<table>
    <tbody>
        <tr>
        <td><img src="images/using_postman_auth_input.png" alt="using_postman_auth_input"></td>      
        </tr>
    </tbody>
</table>

###3. Select "POST" in the dropdown list located above the tabs. 
```Method: POST```
<table>
    <tbody>
        <tr>
        <td><img src="images/using_postman_dropdown_request.png" alt="using_postman_dropdown_request"></td>      
        </tr>
    </tbody>
</table>

###4. Input the request URL path.
```http://msg.rpdata.com/ttsvr/msg?```
<table>
    <tbody>
        <tr>
        <td><img src="images/using_postman_url_request_path.png" alt="using_postman_url_request_path"></td>      
        </tr>
    </tbody>
</table>

###5. Under the "Body" tab, choose "raw". Then select "JSON(application/json)" in the dropdown list.
```Request Body: raw
Data Type: JSON(application/json)```
<table>
    <tbody>
        <tr>
        <td><img src="images/using_postman_body.png" alt="using_postman_body"></td>      
        </tr>
    </tbody>
</table>



###Note:
After Step 5, the "Headers" tab should be automaticaly updated with the following sample;
```Authorization: Basic bXNnOkU3bVc6JTZ7REs=
Content-Type: application/json```
<table>
    <tbody>
        <tr>
        <td><img src="images/using_postman_headers_input.png" alt="using_postman_headers_input"></td>      
        </tr>
    </tbody>
</table>


The input box under the "Boby" tab is where you place the request parameters. 
See sample below;
```{
    "op": "getMobilePropertyAdditionalInfo",
    "uid": "TWISTUSER001",
    "sid": "2-4eed242594fc464787b8054ddc77de11",
    "propertyId": "7764519"
}```
<table>
    <tbody>
        <tr>
        <td><img src="images/using_postman_body_paramaters.png" alt="using_postman_body_paramaters"></td>      
        </tr>
    </tbody>
</table>
