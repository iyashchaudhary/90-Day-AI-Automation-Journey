1- crud and http methods 
| Kaam | Method | Example endpoint |
|---|---|---|
| Create (naya banana) | POST | POST /todos |
| Read (dekhna) | GET | GET /todos, GET /todos/12 |
| Update (badalna) | PUT / PATCH | PATCH /todos/12 |
| Delete (hatana) | DELETE | DELETE /todos/12 |

2- rules 
URL mein noun (resource) aata hai: /todos, /users
- Kaam method batata hai, URL nahi
- Naya banate waqt number nahi, server khud id deta hai
- PUT = poora badalna, PATCH = sirf ek field
3 - path vs query 
query - specific koo filter krne kai liye ex-/posts?userId=1
path - in url btata hai which item ex- /users/5 
