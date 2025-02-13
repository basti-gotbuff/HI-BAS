<form class="form">
  <p class="title">Register</p>
  <p class="message">Signup now and get full access to our app.</p>
  <div class="flex">
    <label>
      <input required="" placeholder="" type="text" class="input" />
      <span>Firstname</span>
    </label>

    <label>
      <input required="" placeholder="" type="text" class="input" />
      <span>Lastname</span>
    </label>
  </div>

  <label>
    <input required="" placeholder="" type="email" class="input" />
    <span>Email</span>
  </label>

  <label>
    <input required="" placeholder="" type="password" class="input" />
    <span>Password</span>
  </label>
  <label>
    <input required="" placeholder="" type="password" class="input" />
    <span>Confirm password</span>
  </label>
  <button class="submit">Submit</button>
  <p class="signin">Already have an acount ? <a href="#">Signin</a></p>
</form>
.form {
  display: flex;
  flex-direction: column;
  gap: 10px;
  max-width: 350px;
  padding: 20px;
  border-radius: 20px;
  position: relative;
  background-color: rgb(255, 166, 0);
  color: #212121;
  border: 1px solid #333333;
}

.title {
  font-size: 28px;
  font-weight: 600;
  letter-spacing: -1px;
  position: relative;
  display: flex;
  align-items: center;
  padding-left: 30px;
  color: #d34d00;
}

.title::before {
  width: 18px;
  height: 18px;
}

.title::after {
  width: 18px;
  height: 18px;
  animation: pulse 1s linear infinite;
}

.title::before,
.title::after {
  position: absolute;
  content: "";
  height: 16px;
  width: 16px;
  border-radius: 50%;
  left: 0px;
  background-color: #d35f00;
}

.message,
.signin {
  font-size: 14.5px;
  color: #333;
}

.signin {
  text-align: center;
}

.signin a:hover {
  text-decoration: underline green;
}

.signin a {
  color: #d3007402;
}

.flex {
  display: flex;
  width: 100%;
  gap: 6px;
}

.form label {
  position: relative;
}

.form label .input {
  background-color: #333;
  color: #fff;
  width: 100%;
  padding: 20px 05px 05px 10px;
  outline: 0;
  border: 1px solid rgba(105, 105, 105, 0.397);
  border-radius: 10px;
}

.form label .input + span {
  color: rgba(255, 255, 255, 0.5);
  position: absolute;
  left: 10px;
  top: 0px;
  font-size: 0.9em;
  cursor: text;
  transition: 0.3s ease;
}

.form label .input:placeholder-shown + span {
  top: 12.5px;
  font-size: 0.9em;
}

.form label .input:focus + span,
.form label .input:valid + span {
  color: #3cd300;
  top: 0px;
  font-size: 0.7em;
  font-weight: 600;
}

.input {
  font-size: medium;
}

.submit {
  border: none;
  outline: none;
  padding: 10px;
  border-radius: 10px;
  color: #0004d3;
  font-size: 16px;
  transform: 0.3s ease;
  background-color: whitesmoke;
  border: 1px solid #00d38d;
}

.submit:hover {
  background-color: #00d370;
  color: whitesmoke;
}

@keyframes pulse {
  from {
    transform: scale(0.9);
    opacity: 1;
  }

  to {
    transform: scale(1.8);
    opacity: 0;
  }
}
