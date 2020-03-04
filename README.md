# PRSSite
The Official Website Of The Phantom Reaper Studios Team

<!-- modify this form HTML and place wherever you want your form -->

<form id="my-form"
  action="https://formspree.io/moqwykpg"
  method="POST"
>
  <label>Email:</label>
  <input type="email" name="email" />
  <label>Message:</label>
  <input type="text" name="message" />
  <button id="my-form-button">Submit</button>
  <p id="my-form-status"></p>
</form>

<!-- Place this script at the end of the body tag -->

<script>
  window.addEventListener("DOMContentLoaded", function() {

    // get the form elements defined in your form HTML above
    
    var form = document.getElementById("my-form");
    var button = document.getElementById("my-form-button");
    var status = document.getElementById("my-form-status");

    // Success and Error functions for after the form is submitted
    
    function success() {
      form.reset();
      button.style = "display: none ";
      status.innerHTML = "Thanks!";
    }

    function error() {
      status.innerHTML = "Oops! There was a problem.";
    }

    // handle the form submission event

    form.addEventListener("submit", function(ev) {
      ev.preventDefault();
      var data = new FormData(form);
      ajax(form.method, form.action, data, success, error);
    });
  });
  
  // helper function for sending an AJAX request

  function ajax(method, url, data, success, error) {
    var xhr = new XMLHttpRequest();
    xhr.open(method, url);
    xhr.setRequestHeader("Accept", "application/json");
    xhr.onreadystatechange = function() {
      if (xhr.readyState !== XMLHttpRequest.DONE) return;
      if (xhr.status === 200) {
        success(xhr.response, xhr.responseType);
      } else {
        error(xhr.status, xhr.response, xhr.responseType);
      }
    };
    xhr.send(data);
  }
</script>

### Site links


[Home](https://phantomreaperstudios.github.io/PRSSite/)  

[Team Members](https://phantomreaperstudios.github.io/PRSSite/Team%20Members/TeamMembers)  

[Art](https://phantomreaperstudios.github.io/PRSSite/Art/Art)




# Wellcome!
Hello if you are reading this that means you are on the PRSSite. Now you are probably wondering what *PRSSite* means well let me tell you. *PRRSite* stands for *Phantom Reaper Studios Site* or *PRSSite* for short. This site is the main and Offical website of *Phantom Reaper Studios*. Now Let me introduce my self. I am the *Founder* and *CEO* of *Phantom Reaper Studios* and I am currently creating this website and ***Github Repository*** so I can share my *Studios* work and projects.

# What We Do And Plan To Do
Well first I think iff you are reading this far your a legend and secondly this is will you will find what we do and what we plan to do.

**What We Do**
Ok now this is what we do. What I hope for this Studio to do is I hope that we can post:

*Art*

*Pixel Art*

*Music*

*Code*

*And More To Come Once We Get More People And Get The Website Made And Running.*

**What We Plan To Do**
Ok this is what we plan to do here at the studio. I hope that we can post all of the above and our most current project is setting up our website and get it ready for the public.

# Who Are We?
Well thats a great question to ask. Well currently it is just me but soon more to come! I am **Phantom Reaper A.K.A MdSn Reaper** and of course I have created this *Studio/Team/Group* what ever you want to call us but I have big hopes to make this become a great community hub and center to have anything and everything!

# Thanks
So That is about all the time I have and I have to go make this website, I am sure glad you read this far. If you have any questions please email the Studio. The contact Information will be below this.

>***-私が誰なのかを教えてくれるので、違うことをあえて***

>***-Dare To Be Different Because Who Am I To Tell Me Who I Am***

>***-The Phantom Reaper***

# How To Contact Us
**Email:** PhantomReaperStudios@gmail.com

**Facebook:** Coming Soon

**Twitter:** Coming Soon
