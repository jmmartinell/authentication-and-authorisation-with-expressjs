# authentication-and-authorisation-with-expressjs
This text has been translated by Meta-Llama-3.1-70B-Instruct.

This repository is part of a learning campaign focused on authentication and authorization in web applications using Express.js.

"Hello. I don't speak English. That's why it wasn't clear to me where to implement the functionality to delete users, whether in the administrators' section or in the users' section. In the end, I decided on the users' section. Changing the implementation of “delete_user_by_username” so that only administrators can use it is very simple, you just need to change “authorisation("user")” to “authorisation("admin")” and change the logic in the view from the file located in “web-front-end\pages\profile.html” to the file located in “web-front-end\pages\admin\dashboard.html”.

Before discussing whether “This delete user functionality can be done after authentication” is a good or bad idea, we need to define Authentication and Authorization.

Authentication: Verify the identity of a user before allowing access.

Authorization: Determine what actions or resources an authenticated user can access.

Now that we have the definitions clear, I think it's a bad idea to allow any user, after authenticating in the system, to execute the delete functionality because they may not have the authorization to do so. Therefore, we must first check if they are authorized to execute this functionality."
