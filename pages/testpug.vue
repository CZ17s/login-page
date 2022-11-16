<template lang="pug">
    v-container.bgimg
      v-row.align-center.justify-center
        v-col(cols="12" md="10")

          v-card.d-flex.justify-center
            v-row
              v-col.bgcard.d-flex.justify-center.flex-column.box.white--text.align-center.rounded-l-xl(cols="12" lg="8" md="12")
                  div.boxtext.d-flex.justify-center.flex-column
                    p.textwellcome Welcome Back !
                    p.textp You can sign in to access with your existing account.
            
              v-col.white.box.d-flex.justify-center.flex-column.align-center.rounded-r-xl(cols="12" lg="4" md="12")
                  div.boxlogin
                    h1.black--text Sign In
                    v-text-field(label="Username or Email" placeholder="" prepend-inner-icon="mdi-email" filled rounded dense )
                    v-text-field(label="Password" placeholder="" prepend-inner-icon="mdi-lock" filled rounded dense )
                    div.d-flex.justify-space-between
                      v-checkbox(label="Remember me")
                      a.d-flex.justify-center.flex-column.black--text Forget Password ?
                  v-btn.btnsize(color="primary" rounded) Sign in
                  div.d-flex.justify-space-between.mt-4
                      p.mr-2 New here?
                      a Create Account
      
  </template>
  
  <script>
  export default {
    name: "testpug",
  };
  </script>
  
  <style>
  .container {
    background-image: url(https://images.pexels.com/photos/114979/pexels-photo-114979.jpeg?cs=srgb&dl=pexels-veeterzy-114979.jpg&fm=jpg);
    background-size: cover;
    height: 100%;
    display: flex;
    justify-content: center;
    flex-direction: column;
  }
  .bgcard{
    background-image: url(https://cdn4.vectorstock.com/i/1000x1000/84/83/abstract-blue-purple-low-poly-background-vector-21528483.jpg);
    width: 700px;
  }
  .box {
    height: 700px;
  }
  
  .boxtext{
    width: 400px;
  }
  .boxlogin{
    width: 300px;
    height: 270px;
  }
  .textwellcome{
    font-size: 55px;
    font-weight: bold;
  }
  .textp{
    font-size: 25px;
  
  }
  .btnsize{
    width: 200px;
  }
  
  </style>
  