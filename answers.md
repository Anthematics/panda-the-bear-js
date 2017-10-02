

Hacking Panda the Bear's Resume

<!-- Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead\ -->

<!-- PROTIP: use the inspector to learn the dimensions of the current profile image and use a placeholder image service such as Place Bear to get an image of the same size. -->

	pic = document.querySelector(".profile-image");
		pic.src = "https://placebear.com/400/400"

<!-- Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing. -->

sky = document.querySelector("#left-image > img");
	sky.src = "https://placebear.com/300/300"
	"https://placebear.com/300/300"
		"https://placebear.com/300/300"


<!-- Select the heading that says "Panda the Bear" and change it to your own name. -->

	heading = document.querySelector("h1.highlight");
		heading.innerText = "Octopus";


<!-- Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector) -->

job = document.querySelector("#employment > h3");
job.innerText = "Job";
"Job";

<!-- Change the colour of the body. document.body or document.querySelector("body") will work the same here-->

	newbody = document.body;
		newbody.style.color = "blue";  
<!-- if i want to change a style I could have changed in css -> call style.(whateveriwanttochange) -->

<!-- Change the colour of each element using the highlight class. Use a for loop to do this. -->
	allele= document.querySelectorAll(".highlight")
		for (var i =0; i < allele.length; i++) {
			allele[i].style.color = "yellow";
	}

"yellow"

<!-- Change the font family of the h1 to 'monospace'. -->

mons = document.querySelector("h1");
mons.style.fontFamily = "monospace";

<!-- Find a way to select the round icons in the sidebar and then change their colour. -->

roundj = document.querySelectorAll(".action-icon-bg")
for (var k =0; k <roundj.length; k++)  {
console.log(k,roundj,roundj[k]);
roundj[k].style.backgroundColor = "blue" ;  
}



<!-- Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself". -->
inform = document.querySelector("#name")
inform.placeholder = "kljsaefefkaeh"
<!-- #= ID's . (period) = class -->

#name.contact-info

<!-- Change the placeholder attribute of the message field to "state your business". -->

message = document.querySelector("#message")
message.placeholder= "State ur business"

<!-- Give the name field a "value" attribute of "your nemesis". -->

nemesis = document.querySelector("#name")
nemesis.defaultValue = "Your Nemesis"
"Your Nemesis"


<!-- Change the value attribute of the email field to "koalathebear@gmail.com". -->
email2 = document.querySelector("#name")
email2.defaultValue = koalathebear@gmail.com

<!-- Change the value of the submit button on the contact form to "En garde!". -->
subbutton = document.querySelector('#submit')
subbutton.defaultValue ="En garde"

<!-- We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute). -->
subbutton1 = document.querySelector('#submit')
subbutton1.disabled ="true"

<!-- We should help Panda protect their privacy by erasing their personal details from the sidebar. -->
hideinfo = document.querySelector(".bio-info")
hideinfo.hidden = "true"
"true"

<!-- That drawing of Pikachu is really cute. Let’s duplicate it using cloneNode() and insert it at the bottom of the .portfolio-container using insertAdjacentHTML() or appendChild(). -->

pikachu = document.querySelector("#right-image > img")
pikachuClone = pikachu.cloneNode(true)

portfolioc = document.querySelector('.portfolio-container')
portfolioc.appendChild(pikachuClone)

<!-- Wow, that was so satisfying I think we should do it 10 more times. Use a for loop to help you do this. -->

<!-- Let’s add a message about when the page was last updated. We'll do this by appending a new <li> element to the <ul> in the sidebar (you might need to refresh the page to bring back the list items that we emptied out earlier). -->





document.createElement, document.createTextNode, and appendChild are the keys to this process.

First we need to construct a new <li> tag.

var listItem = document.createElement('li');

It isn't part of the DOM yet, it's just floating in the void. We'll eventually attach it to the <ul> in the sidebar, below Panda's name, location, and phone number.

Now we need a new <span> tag to go inside the <li> we just made. This span will eventually go in the left column below 'Phone'.

var leftSpan = document.createElement('span');

Next we need to make a "text node" in order to put text inside our new span. A text node is a chunk of plain text that lives inside some HTML tag in the DOM.

var lastUpdated = document.createTextNode('Page last updated on');

We're ready to put that new text node inside our new <span> using appendChild.

leftSpan.appendChild(lastUpdated);

And we'll put the <span> inside the <li>, again using appendChild.

listItem.appendChild(leftSpan);

At this point our new elements are attached to each other but are still floating in the void separate from our webpage's DOM.

It's up to you to go through the same process for the second span that will go in the right-hand column of the <ul> (below Panda's phone number). Look up the docs for the Date class to find a way of displaying the current date inside your next text node.

After that, find a way of selecting the <ul> and append the new <li> to it. For bonus marks, apply the correct classes to these new elements of yours so the styling is consistent with the rest of the list items.
