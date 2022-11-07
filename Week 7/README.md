# Writing Week 6
## **React Router**

- **Prop Types**
- PropTypes merupakan sebuah library yang dapat membantu dalam memeriksa tipe data props yang apabila tidak sesuai maka akan memunculkan pesan error
- Contoh code 
  ```
  import React from 'react';
  import PropTypes from 'prop-types';
  const User = (props) => {
  const {hobby} = props;
  return (
    <>
      <h1>My hobby is {hobby}</h1>
    </>
  );
  };
  export default function App() {
  return (
    <div>
      <h1>Hello Alwan</h1>
      <User hobby="Playing games" />
    </div>
    );
  }
  User.propType = {
  name: PropTypes.string
  };
  ```
### **Router**
- React Router merupakan standar library untuk routing pada React.
- standar routing berfungsi untuk membuat suatu website menjadi dynamic.
- Pada React, Router membantu untuk mengarahka page satu ke page yg lainnya berdasarkan path url yg ditentukan.
- Cara menginstall/menggunakan React Router : 
  - npm install react-router-dom
  - Menambahkan import { BrowserRouter } from "react-router-dom"; pada bagian index.js
  - Menambahkan code :
  ```
   <BrowserRouter>
      <App />
    </BrowserRouter>
  ```
- Browser Router merupakan interface pada umumnya yg digunakan  untuk menjalankan react di browser atau untuk membuat router-router sederhana.
- HashRouter penulisannya menggunakan #, yg digunakan pada sebuah website yang menggunakan satu page saja.
- Code pada Bagian App.js
  ```
  import React from 'react'
  import { BrowserRouter, Route, Switch } from 'react-router-dom'

  import Home from './pages/Home'
  import Profil from './pages/Profil'
  import ProfilDetail from './pages/ProfilDetail'

  function App() {
    return (
      <BrowserRouter>
        <Switch>
          <Route path="/" exact component={Home} />
          <Route path="/profil" exact component={Profil} />
          <Route path="/profil/:name" exact component={ProfilDetail} />
        </Switch>
      </BrowserRouter>
    )
  }

  export default App
  ```
- Code pada Bagian Page Home
  ``` 
  import React from 'react'
  import { Link } from 'react-router-dom'

  function Home(props) {
    return (
      <>
        <h2>
          Home page
        </h2>

        <Link to="/profil">Menuju profil</Link>
      </>
    )
  }
  ```
- 3 cara penggunaan router :
  - Routing Dasar
  - Dynamic Route
  - Nested Route
  
### **React Redux**
- Redux adalah library JavaScript yang digunakan untuk mengelola state pada
aplikasi React. Redux memiliki beberapa kelebihan antara lain:

  1. Redux memudahkan kita untuk mengelola state pada aplikasi React.
  2. Redux memudahkan kita untuk mengelola state pada aplikasi React yang
   kompleks.
  3. Redux memudahkan kita untuk mengelola state pada aplikasi React yang berskala
   besar.
  4. Redux memudahkan kita untuk mengelola state pada aplikasi React yang berskala
   besar dan kompleks.
  5. Redux memudahkan kita untuk mengelola state pada aplikasi React yang berskala
   besar dan kompleks dengan banyak pengguna.

- Yaitu dengan menyimpan state di satu tempat, sehingga lebih mudah untuk di manage.
- cara kerja Redux :
  - Action : Adalah sebuah function yang mereturn sebuah objek.
  - Reducer : sebuah fungsi yang tugasnya untuk mengolah state yang ada di store.
  - Store : tempat untuk menampung state

### Redux-Thunk
- Redux-Thunk adalah sebuah middleware yang memungkinkan kita memanggil pembuat aksi yang mengembalikan fungsi sebagai ganti objek aksi.
- Redux-Thunk solusi ketika kita menggunakan fetch data dari sebuah External API atau yang memiliki side effect (proses ashynchronous).
- Installation Redux-Thunk
```jsx
npm install redux react-redux redux-thunk
```
