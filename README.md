# -LT-13_Tipe_Data_Object

Object adalah tipe data yang digunakan untuk menyimpan dan mengelola sekumpulan pasangan nilai-kunci (key-value). Setiap pasangan nilai-kunci dalam object disebut property, dan nilai dari property tersebut disebut dengan value. Property dapat berupa tipe data apa saja, baik itu tipe data primitif (seperti number, string, dan boolean) maupun tipe data objek (seperti object dan array). Contoh:

    let user = {
      name: "John",
      age: 30,
      isAdmin: true
    };

    console.log(user.name); // output: "John"
    console.log(user.age); // output: 30
    console.log(user.isAdmin); // output: true

Anda juga dapat mengakses property dalam object menggunakan operator kurung siku ([]). Contoh:

    let user = {
      name: "John",
      age: 30,
      isAdmin: true
    };

    let key = "name";
    console.log(user[key]); // output: "John"

    key = "age";
    console.log(user[key]); // output: 30

    key = "isAdmin";
    console.log(user[key]); // output: true

Selain property yang berisi tipe data primitif atau objek, object juga dapat memiliki property yang berisi function. Property yang berisi function disebut dengan method. Anda dapat menjalankan method dengan menggunakan operator titik (.) atau kurung siku ([]). Contoh:

    let user = {
      name: "John",
      age: 30,
      sayHello: function() {
        console.log(`Hello, my name is ${this.name}`);
      }
    };

    user.sayHello(); // output: "Hello, my name is John"

    let key = "sayHello";
    user[key](); // output: "Hello, my name is John"

Anda dapat menambah atau mengubah property atau method pada object dengan menggunakan operator titik (.) atau kurung siku ([]). Contoh:

    let user = {
      name: "John",
      age: 30
    };

    user.email = "john@example.com";
    console.log(user.email); // output: "john@example.com"

    user["isAdmin"] = true;
    console.log(user.isAdmin); // output: true

    user.sayHello = function() {
      console.log(`Hello, my name is ${this.name}`);
    };
    user.sayHello(); // output: "Hello, my name is John"

