In this project, let's build a **Prime Video** by applying the concepts we have learned till now.

### Refer to the video below:

<br/>
<div style="text-align: center;">
  <video style="max-width:80%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12);outline:none;" loop="true" autoplay="autoplay" controls="controls" muted>
    <source src="https://assets.ccbp.in/frontend/content/react-js/prime-video-output.mp4" type="video/mp4">
    
  </video>
</div>
<br/>

### Design Files

<details>
<summary>Click to view</summary>

- [Large (Size >= 992px) and Extra Large (Size >= 1200px)](https://assets.ccbp.in/frontend/content/react-js/prime-video-lg-output-img.png)

</details>

### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>
<summary>Functionality to be added</summary>
<br/>

The app must have the following functionalities

- **Action Movies List** and **Comedy Movies List** should be displayed using **React Slick**
- The `App` is provided with `moviesList`. It consists of a list of movieItem objects with the following properties in each movieItem object

  |     Key      | Data Type |
  | :----------: | :-------: |
  |      id      |  String   |
  | thumbnailUrl |  String   |
  |   videoUrl   |  String   |
  |  categoryId  |  String   |

- When the **next button** is clicked in any of the sliders, the next movie items thumbnail in the corresponding moviesList should be displayed
- When the **previous button** is clicked in any of the sliders, the previous movie items thumbnail in the corresponding moviesList should be displayed <br/>

  <div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/prime-video-next-previous-buttons-img.png" alt="movie slider buttons" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
  </div>
<br/>

- When you click on the **thumbnail**, then the popup should be opened,

  - And corresponding video should be displayed using **React player** component from `react-player`
    <div style="text-align: center;">
      <img src="https://assets.ccbp.in/frontend/content/react-js/prime-video-popup-img.png" alt="popup" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
  </div>
  <br/>
  - When the close button is clicked, then the popup should be closed

</details>

<details>
<summary>Components Structure</summary>

<br/>
<div style="text-align: center;">
    <img src="https://assets.ccbp.in/frontend/content/react-js/prime-video-compoment-structure-breakdown.png" alt="component structure breakdown" style="max-width:100%;box-shadow:0 2.8px 2.2px rgba(0, 0, 0, 0.12)">
</div>
<br/>

</details>

<details>
<summary>Implementation Files</summary>
<br/>

Use these files to complete the implementation:

- `src/components/PrimeVideo/index.js`
- `src/components/PrimeVideo/index.css`
- `src/components/MoviesSlider/index.js`
- `src/components/MovieItem/index.js`
- `src/components/MovieItem/index.css`

</details>

### Quick Tips

<details close>
<summary>Click to view</summary>

- To build this project, take a look at the <a href='https://learning.ccbp.in/frontend-development/course?c_id=2f4192f7-7495-49ca-a6ce-6b74005e25f1&s_id=c1dc8b6e-864b-4417-9767-471b9e745405&t_id=416f0cab-8425-413b-9157-c7b4d4ae4467' target="_blank">React Slick</a>, <a href='https://learning.ccbp.in/frontend-development/course?c_id=2f4192f7-7495-49ca-a6ce-6b74005e25f1&s_id=b01fca1c-aa5c-4d79-b81e-0220e7649bd0&t_id=416f0cab-8425-413b-9157-c7b4d4ae4467' target="_blank">React Popup</a> and <a href='https://learning.ccbp.in/frontend-development/course?c_id=2f4192f7-7495-49ca-a6ce-6b74005e25f1&s_id=b6392b63-25f6-4215-be09-9f23ad91d789&t_id=416f0cab-8425-413b-9157-c7b4d4ae4467' target="_blank">React Video Player</a> reading materials

- To style popup content use `.popup-content` class

```jsx
<Popup
  modal
  trigger={
    //write code here
  }
  className="popup-content"
>
  //write code here
</Popup>
```

</details>

### Important Note

<details>
<summary>Click to view</summary>

<br/>

**The following instructions are required for the tests to pass**

- One frame of the slider should have 4 thumbnails
- The thumbnail images in the app should have alt as **thumbnail**
- The close button in the popup should have the `data-testid` as **closeButton**
- `IoMdClose` from react-icons should be used for **Close Icon** in the Popup

</details>

### Resources

<details>
<summary>Image URLs</summary>

- [https://assets.ccbp.in/frontend/react-js/prime-video-img.png](https://assets.ccbp.in/frontend/react-js/prime-video-img.png) alt should be **prime video**

</details>

<details>
<summary>Colors</summary>

<br/>
<div style="background-color: #000000; width: 150px; padding: 10px; color: white">Hex: #000000</div>
<div style="background-color: #ffffff; width: 150px; padding: 10px; color: black">Hex: #ffffff</div>
<div style="background-color: #231f20; width: 150px; padding: 10px; color: white">Hex: #231f20</div>
<br/>

</details>

<details>
<summary>Font-families</summary>

- Roboto

</details>

> ### _Things to Keep in Mind_
>
> - All components you implement should go in the `src/components` directory.
> - Don't change the component folder names as those are the files being imported into the tests.
> - **Do not remove the pre-filled code**
> - Want to quickly review some of the concepts you’ve been learning? Take a look at the Cheat Sheets.
