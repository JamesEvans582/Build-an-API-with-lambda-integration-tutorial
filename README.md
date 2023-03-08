# Build-an-API-with-lambda-integration-tutorial
AWS tutorial

Firstly we will need to go to Lambda then create function.

<img width="1792" alt="Screenshot 2023-02-11 at 07 46 40" src="https://user-images.githubusercontent.com/71371405/218247746-3d294891-ec04-4265-bd6f-09b65b01c85f.png">

In function name call it what you like. For me I followed this tutorial off whizlabs so I used theirs. 
Run time click on the drop down and enter python 3.8

Change the execution role to create a new role with AWS policy templates.
<img width="1792" alt="Screenshot 2023-02-11 at 07 47 18" src="https://user-images.githubusercontent.com/71371405/218247861-50fe749e-3770-4c83-9146-0d51d493de0c.png">
Enter your role new with API. Then choose Basic Lambda@edge permissions (for cloudfront trigger)

Then hit create! 

![screenshot_129](https://user-images.githubusercontent.com/71371405/218248070-8d0df6d2-297f-425f-a428-e2fcf403097f.png)

Well done so far. Now we need to create the API. So on the console, go to API gateway, then build.
<img width="1792" alt="Screenshot 2023-02-11 at 07 51 23" src="https://user-images.githubusercontent.com/71371405/218248235-4f45bad0-fb8a-45c1-b9c2-5c3da5cf7563.png">

It will then give you an option of the types of API. We'll choose RestAPI, the third option, not the VPC, that's not needed for this tutorial.

So now we need to create the resource. Click actions then create resource.  
<img width="1792" alt="Screenshot 2023-02-11 at 07 54 12" src="https://user-images.githubusercontent.com/71371405/218248486-9343e697-c7d2-419b-a6a0-b0e86eace191.png">
Type in the resource name, then click create resource. 

That's great, we have resource but what action does it take, and how? This is where we create a method. So once again click action. We will put in the name and use a GET method, then click create.

Once you have done these stages, you're nearly there. So lets click on Deploy API

<img width="1792" alt="Screenshot 2023-02-11 at 07 59 47" src="https://user-images.githubusercontent.com/71371405/218249184-bf7f954b-bac0-45a7-ab07-5153c51b6390.png">

In the deployment stage enter new, then enter the stage name, we're testing, so put testing API, and enter a brief description and deploy.

Final stage we need to invoke the URL and make sure the API is connecting to Lamda.
<img width="1792" alt="Screenshot 2023-02-11 at 08 02 05" src="https://user-images.githubusercontent.com/71371405/218249428-2ab9015c-f03c-45d7-8973-714c1a1c628d.png">

Click the link. Which will take you to a browser. You need to /whizlabsapi to test that it has validated. If it has it should look like the picture below.
<img width="1792" alt="Screenshot 2023-02-11 at 08 05 36" src="https://user-images.githubusercontent.com/71371405/218249566-2dbe1d45-9111-474f-9f7f-75717bee71b0.png">

Status 200 code, which means it sucessfully been created and a little texed from Lambda to. 

That's all she wrote, hoped you found this tutorial helpful.

Happy clouding.





