API Documentation

Example Axios Request for LOGIN:

A POST that takes in an email and password for authentication.

Example Request:
const result = await axios({
        method: 'post',
        url: 'https://secret-brook-97060.herokuapp.com/login',
        data:{
            "email": email,
            "password": password ,
        },
        withCredentials: true
    });
    
    
    
    
    
Example Axios Request for SIGNUP:

A POST that requires an email, password, and preferences to store in backend user signs up with an account.

Example Request:
const result = axios({
        method: 'post',
        url: 'https://secret-brook-97060.herokuapp.com/signuppage',
        data:{
            "email":email,
            "password": password,
            "preferences": preferences
        },
    })
    
    


Example Axios Request for remembering signed in user:

A GET that retrieves the currently signed in user. 

Example Request:
const result = axios({
        method: 'get',
        url: 'https://secret-brook-97060.herokuapp.com/',
        withCredentials: true
    });
    
    
    
Example Axios Request for when the user decided to LOG OUT.

A GET that logs the user out by clearing the saved session.

const result = axios({
        method: 'get',
        url: 'https://secret-brook-97060.herokuapp.com/logout',
        withCredentials: true
    });
    
    
    
