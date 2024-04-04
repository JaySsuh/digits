<h1>Digits-semantic-ui</h1>
<img src="doc1/landing.png">
<p>Digits is an application that allows users to:</p>
<ul>
<li>Register an account</li>
<li>Create and manage a set of contacts.</li>
<li>Add a set of timestamped notes regarding their interactions with each contact.</li>
</ul>
<h2 class="red-text" style="color: red">Installation</h2>
<p>First, install Meteor</p>
<p>Second, download a copy of Digits. Note that Digits is a private repo and so you will need to request permission from the author to gain access to the repo.</p>
<p>Third, cd into the app directory install the required libraries with:</p>
<img src="doc1/meteornpm.png">
<p>Once the libraries are installed, you can run the application by invoking:</p>
<img src="doc1/meteornpmrun.png">
<p>The first time you run the app, it will create some default users and data. Here is the output:</p>
<img src="doc1/firststart.png">
<p>On some operating systems (particularly Windows), installing bcrypt is much more difficult than implied by the above message. Bcrypt is only used in Meteor for password checking, so the performance implications are negligible until your site has very high traffic. You can safely ignore this warning without any problems during initial stages of development.

If all goes well, the template application will appear at http://localhost:3000. You can login using the credentials in settings.development.json, or else register a new account.

Lastly, you can run ESLint over the code in the imports/ directory with:</p>
<img src="doc1/meteorlint.png">
<h2>User Interface Walkthrough</h2>
<h4>Landing Page</h4>
<p>When you first bring up the application, you will see the landing page that provides a brief introduction to the capabilities of Digits:</p>
<img src="doc1/landing.png">
<h4>Register</h4>
<p>If you do not yet have an account on the system, you can register by clicking on “Login”, then “Sign Up”:</p>
<img src="doc1/reg.png">
<h4>Sign in</h4>
<p>Click on the Login link, then click on the Signin link to bring up the Sign In page which allows you to login:</p>
<img src="doc1/signin.png">
<h4>User home page</h4>
<p>After successfully logging in, the system takes you to your home page. It is just like the landing page, but the NavBar contains links to list contact and add new contacts:</p>
<img src="doc1/john.png">
<h4>List Contacts</h4>
<p>Clicking on the List Contacts link brings up a page that lists all of the contacts associated with the logged in user:</p>
<img src="doc1/list.png">
<p>This page also allows the user to add timestamped “notes” detailing interactions they’ve had with the Contact. For example:</p>
<img src="doc1/note.png">
<h4>Edit Contacts</h4>
<p>From the List Contacts page, the user can click the “Edit” link associated with any Contact to bring up a page that allows that Contact information to be edited:</p>
<img src="doc1/edit.png">
<h4>Admin mode</h4>
<p>It is possible to designate one or more users as “Admins” through the settings file. When a user has the Admin role, they get access to a special NavBar link that retrieves a page listing all Contacts associated with all users:
</p>
<img src="doc1/admin.png">