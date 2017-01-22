## OneHourTranslation API-2 Methods and Environment for Postman #

### Introduction 

One Hour Translation&trade; provides translation, proofreading and transcription services worldwide.
The following API library allows customers to submit and monitor jobs automatically and remotely.

### Preconditions

#### Authentication 
1. Register as a customer on [One Hour Translation](http://www.onehourtranslation.com/auth/register).
2. Request your API Keys [here](http://www.onehourtranslation.com/profile/apiKeys).
3. [Download](https://www.getpostman.com/) Postman app.

#### Add OneHourTranslation methods
![optimised1](https://cloud.githubusercontent.com/assets/18589621/22182624/7d7cc70e-e0b2-11e6-9e43-0a1c7eb6443d.gif)

1. Click on import button in the upper-left corner.
2. Drag or choose "OneHourTranslation API V2.json" collection file.

Methods will appear in the left section of the app.

#### Add OneHourTranslation Environment
![optimised3](https://cloud.githubusercontent.com/assets/18589621/22182628/8bd8b42a-e0b2-11e6-89d8-67f8fd6ce6bb.gif)

1. Click on the gear icon at the upper-right corner.
2. Select Manage Environment from the drop down menu.
3. Click on import.
4. Select "OneHourTranslation Environment.json" file

#### Add account information to your environment
![optimised2](https://cloud.githubusercontent.com/assets/18589621/22182627/856d4ef2-e0b2-11e6-9b41-87b3c6699898.gif)

1. Click on the gear icon at the upper-right corner.
2. Select Manage Environment from the drop down menu.
3. Select imported environment.
4. Enter your secret key.
5. Enter your public key.
6. Enter API URL, if you want to use live account enter http://www.onehourtranslation.com/api/2, if you want to test API methods in the sandbox simulated site enter https://sandbox.onehourtranslation.com/api/2.
7. Enter callback URL, if you have a callback URL enter it here if not leave blank.

* Make sure you are entering the right authentication keys, live site keys won't work in sandbox and sandbox keys won't work in live site.

### Making API Calls
Secret and public keys are taken from the environment setup automatically, no need to enter them again.

#### Execute GET calls
Select a Get call like "Get Resource Content", to see the needed params click on "Params" button at the top:
![image](https://cloud.githubusercontent.com/assets/18589621/22182784/60e3c7ce-e0b6-11e6-99c6-e954d15c6c4e.png)

There are two kinds of parameters you need to add to a get call:

1. Parameters like project_id, resource_uuid those are edited in the url:
![image](https://cloud.githubusercontent.com/assets/18589621/22182800/d212f3fc-e0b6-11e6-9da8-53c744dd4d35.png)

2. Parameters that will be transferred with the GET method:
![image](https://cloud.githubusercontent.com/assets/18589621/22182809/fd5a0a50-e0b6-11e6-99a9-647ec5c51099.png)

* Once all parameters are added click on "Send" button and the call will be executed.
In order for the call to execute correctly, you need to enter valid values in those fields.

#### Execute POST Calls
In POST calls there are some methods which like in the GET methods need a parameter in the url, like the "Post a New Comment" method. User needs to specify project id:
![image](https://cloud.githubusercontent.com/assets/18589621/22182833/b0b8fd04-e0b7-11e6-8f0c-8bccb290e395.png)

##### Create a new translation project

1. Select "New Translation Project"
2. Click on "Body" tab to see required parameters:
![image](https://cloud.githubusercontent.com/assets/18589621/22182843/198d9d8a-e0b8-11e6-9969-abed7a284d07.png)

3. Enter all required params. For more information please refer to [OneHourTranslation API](https://www.onehourtranslation.com/translation/api-documentation-v2/general-instructions).
4. Optional parameters in postman turned off in the collection to add an optional parameter to the call check the check-box on the left of the parameter. Example - If we want to add a "wordcount" parameter to our call we will check the check-box and add a value to the param:

  Before:
  ![image](https://cloud.githubusercontent.com/assets/18589621/22182877/ed8e71ea-e0b8-11e6-8b1f-cb96ddf408ed.png)
  
  After:
  ![image](https://cloud.githubusercontent.com/assets/18589621/22182883/0cdf5f32-e0b9-11e6-9bd3-ed84cbadcdc9.png)
  
5. Once all parameters are added click on "Send" button and the call will be executed.
