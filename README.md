# Portfolio_Yogesh_Jha

Created my own portfolio project using HTML, CSS and Javascript. Connected the contact form using Google Excel sheet.<br/>
Also, This portolio is live and hosted through gitHub.<br/>



Here is the code through which I connected my contact me form using excel:👇🏻<br/>

const scriptURL = 'Your google sheet link'<br/>
const form = document.forms['submit-to-google-sheet']<br/>
const msg = document.getElementById("msg")<br/>

form.addEventListener('submit', e => {<br/>
  e.preventDefault()<br/>
  fetch(scriptURL, { method: 'POST', body: new FormData(form)})<br/>
    .then(response => {<br/>
        msg.innerHTML = "Message Sent successfully"<br/>
        setTimeout(function(){<br/>
            msg.innerHTML = ""<br/>
        },5000)<br/>
        form.reset()<br/>
    })<br/>
    .catch(error => console.error('Error!', error.message))<br/>
})<br/>



If you want detail how to connect it through this code, just message me through linkedin or through my contact me form given inside the portfolio.<br/>

Sample of UI (Portfolio) given below👇🏻<br/>

![Screenshot (541)](https://github.com/Yogesh-160/Portfolio_Yogesh_Jha/assets/124399567/b062f71a-1aeb-46cd-9f19-921f3540fdcf)<br/>


Link to access my portfolio 👉🏻 https://yogesh-160.github.io/Portfolio_Yogesh_Jha/<br/>


Connect with me on Linkedin if you have any query regarding my project.  <br/>
OR<br/>
Simply fill the contact me form which is given inside my portfolio project.<br/>


Give start if you love my hardwork ⭐️<br/>