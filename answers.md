# Panda The Bear Answers

1. Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.
```
profile = document.querySelector('.profile-image');
profile.src = 'https://placebear.com/400/400';
```
  1. Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.
  '''
  s = document.querySelector('#left-image').firstElementChild
  s.src = 'https://picsum.photos/325/225';
  ```

2. Select the heading that says "Panda the Bear" and change it to your own name.
```
h = document.querySelector('h1');
h.innerText = 'Jessica';
```

3. Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)
```
e = document.querySelector('#employment').querySelector('h3');
e.innerText = 'Experience';
```

4. Change the colour of the body.
```
b = document.querySelector('body');
b.style.background = '#006266';
```

5. Change the colour of each element using the highlight class. Use a for loop to do this.
```
highlight = document.querySelectorAll('.highlight');
highlight.forEach((element) => {
    element.style.color = "#006266";
});
```

6. Change the font family of the h1 to 'monospace'.
```
document.querySelector('h1').style.fontFamily = "monospace";
```

7. Find a way to select the round icons in the sidebar and then change their colour.
```
round_icons = document.querySelectorAll('.action-icon-bg');
round_icons.forEach((icon) => {
    icon.style.background = '#006266';
});
```

8. Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".
```
document.querySelector('#name').placeholder = 'Identify yourself';
```

9. Change the placeholder attribute of the message field to "state your business".
```
document.querySelector('#message').placeholder = 'State your business.';
```

10. Give the name field a "value" attribute of "your nemesis".
```
document.querySelector('#name').value = 'Your nemesis';
```

11. Change the value attribute of the email field to "koalathebear@gmail.com".
```
document.querySelector('#email').value = 'koalathebear@gmail.com';
```

12.  Change the value of the submit button on the contact form to "En garde!".
```
document.querySelector('#submit').value = 'En garde!';
```

13. We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).
```
document.querySelector('#submit').disabled = true;
```

14. We should help Panda protect their privacy by erasing their personal details from the sidebar.
```
bio = document.querySelector('.bio-info');
parent = bio.parentElement;
parent.removeChild(bio);
```