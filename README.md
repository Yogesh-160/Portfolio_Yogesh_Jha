# Portfolio_Yogesh_Jha

Created my own portfolio project using HTML, CSS and Javascript. Connected the contact form using Google Excel sheet.
Also, This portolio is live and hosted through gitHub.



Here is the code through which I connected my contact me form using excel:👇🏻

const scriptURL = 'Your google sheet link'
const form = document.forms['submit-to-google-sheet']
const msg = document.getElementById("msg")

form.addEventListener('submit', e => {
  e.preventDefault()
  fetch(scriptURL, { method: 'POST', body: new FormData(form)})
    .then(response => {
        msg.innerHTML = "Message Sent successfully"
        setTimeout(function(){
            msg.innerHTML = ""
        },5000)
        form.reset()
    })
    .catch(error => console.error('Error!', error.message))
})



If you want detail how to connect it through this code, just message me through linkedin or through my contact me form given inside the portfolio.

Sample of UI (Portfolio) given below👇🏻

![Screenshot (541)](https://github.com/Yogesh-160/Portfolio_Yogesh_Jha/assets/124399567/b062f71a-1aeb-46cd-9f19-921f3540fdcf)


Link to access my portfolio 👉🏻 https://yogesh-160.github.io/Portfolio_Yogesh_Jha/


Connect with me on Linkedin if you have any query regarding my project.  
OR
Simply fill the contact me form which is given inside my portfolio project.


Give start if you love my hardwork ⭐️