<template>
    <div class="login-page">
      <NuxtPage/>
      <form>
        <h1>Login</h1>
        <div class="form-group">
          <label for="username">Username:</label>
          <input type="text" id="username" name="username" required>
        </div>
        <div class="form-group">
          <label for="password">Password:</label>
          <input type="password" id="password" name="password" required>
        </div>
        <div class="form-group">
          <button type="submit">Login</button>
        </div>
      </form>
      <TableView/>
    </div>
  </template>

  <script>
import TableView from './TableView.vue'
    export default{                    
        name: 'Demo',
        components: {
        TableView
        },
    }
</script>
  
  <style>
  .login-page {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  
  form {
    border: 1px solid #ccc;
    border-radius: 5px;
    padding: 20px;
  }
  
  h1 {
    text-align: center;
  }
  
  .form-group {
    margin-bottom: 20px;
  }
  
  label {
    display: block;
    margin-bottom: 5px;
  }
  
  input[type="text"], input[type="password"] {
    border: 1px solid #ccc;
    border-radius: 5px;
    padding: 5px;
    width: 100%;
  }
  button[type="submit"] {
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
    padding: 10px 20px;
    cursor: pointer;
    width: 100%;
  }
  </style>
  