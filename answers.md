

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

pikachu = document.querySelector("#right-image > img")


portfolioc = document.querySelector('.portfolio-container')

for (var pika =0; pika < 10; pika++)  {
	pikachuClone = pikachu.cloneNode(true);
portfolioc.appendChild(pikachuClone);  
}

<!-- Let’s add a message about when the page was last updated. We'll do this by appending a new <li> element to the <ul> in the sidebar (you might need to refresh the page to bring back the list items that we emptied out earlier). -->

var listItem = document.createElement('li');
var leftSpan = document.createElement('span');
var lastUpdated = document.createTextNode('Page last updated on');
leftSpan.appendChild(lastUpdated;)
listItem.appendChild(leftSpan);
