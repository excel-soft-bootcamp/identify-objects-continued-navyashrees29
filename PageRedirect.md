# Redirect from one page to another in asp.net

- Response.Redirect
- Server.Transfer
- Server.Exceute
- Cross page posting

# Response.Redirect
It redirects a client to a new URL. Specifies the new URL and whether execution of the current page should terminate.

Example : 

protected void Button1_Click(object sender, EventArgs e)
{
Response.Redirect("page1.aspx"); 
}

# Server. Transfer

It is a navigation technique in an ASP.NET web application to move from one web form to another on the same server without changing the URL in an address bar.

Example : 

protected void Button1_Click(object sender, EventArgs e)
{
Server.Transfer("page1.aspx"); 
}

# Server.Exceute

It is also a navigation technique similar to server.transfer but has a different behavior when doing the process.When using the server.
Exceute method for navigation it helps to retain the execution control from the source web form.

Example : 

protected void Button1_Click(object sender, EventArgs e)
{
Server.Execute("WebForm1.aspx");  
}

# Cross Page posting

In an ASP.NET web form is the default page posted on itself whenever a button is clicked.

The Cross Page posting technique allows a web form to post on another web form on button click. The PostbackUrl 
property of the button is set to the page where you want to do cross-page posting.
