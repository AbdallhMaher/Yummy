# Yummy
Welcome to Yummy, your ultimate destination for exploring a wide variety of delicious recipes from around the world. Whether you're looking for a quick meal idea or an elaborate dish for a special occasion, we've got you covered.

## Features

- **Search**: Quickly find recipes or food-related content with our efficient search functionality.
- **Categories**: Browse through a diverse range of food categories to discover recipes that suit your taste.
- **Area**: Explore dishes from different regions and cuisines, bringing global flavors to your kitchen.
- **Ingredients**: Search for recipes based on specific ingredients you have at home, making meal planning a breeze.
- **Contact Us**: Reach out to us for any inquiries, suggestions, or support.

## Getting Started
This project is a starting point for Front-End Applications.

To get started with Culinary Delight:

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdallhMaher/Yummy.git
   cd Yummy
2. Open the project in your preferred code editor.

3. Run project on live server
## project view
<img src="images/Screenshot 2024-07-29 052607.png"  >
  
<img src="images/Screenshot 2024-07-29 052533.png"  >

<img src="images/Screenshot 2024-07-29 052645.png"  >

<img src="images/Screenshot 2024-07-29 052715.png"  >


### java script code for getmeal


``` 
async function getmeal(){
  $(".inn-load").fadeIn(300);
let meals=await fetch(`https://www.themealdb.com/api/json/v1/1/categories.php`)
 meals= await meals.json();
let listmeal = meals.categories;
displycato(listmeal);
$(".items").click(function(e){
 let ix=  $(e.target).attr("count");
 getCategoryMeals(listmeal[ix].strCategory)
}
```

### side navbar

```
<div class="side-nav-menu min-vh-100 position-fixed d-flex top-0">
    <div class="nav-tab  min-vh-100 ">
    <div class="p-4 d-flex flex-column justify-content-between min-vh-100 ">
    <div class="links">
        <ul class="list-unstyled overflow-hidden">
            <li  class="py-2 position-relative cursor-pointer" id="ser">Search</li>
            <li class="py-2 position-relative cursor-pointer" id="cat">Categories</li>
            <li  class="py-2 position-relative cursor-pointer" id="are">Area</li>
            <li  class="py-2 position-relative cursor-pointer" id="ING">Ingredients</li>
            <li  class="py-2 position-relative cursor-pointer" id="con">Contact Us</li>
        </ul>
    </div>
    <div class="nav-footer">
        <div class="icons">
            <i class="fa-brands fa-facebook"></i>
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-solid fa-globe"></i>
        </div>
        <div class="footer">
            <p>Copyright Â© 2019 All Rights <br>Reserved.</p>
        </div>
    </div>
</div>
    </div>
    <div class="nav-header d-flex flex-column justify-content-between py-4 text-center px-2 bg-white text-black">
        <img class="logo" src="Screenshot 2023-03-16 184344.png" alt="" srcset="">
        <i id="icon" class="fa-solid open-close-icon fa-bars fa-2x"></i>
        <div>
            <i class="fa-solid fa-globe d-block"></i>
            <i class="fa-solid fa-share-nodes"></i>
        </div>
    </div>
</div>
```

## Additional Information


**Social Media Links**: Connect with us on social media for more updates and food inspiration. Follow us on [Facebook](https://www.facebook.com/aljnrlabdullah.aljnrlabdullah) -facebook profile and [Instagram](https://www.instagram.com/abdllah_maher00/) - instagrm profile.

## Contact

For any questions or feedback, please contact me at ma4968867@gmail.com.
