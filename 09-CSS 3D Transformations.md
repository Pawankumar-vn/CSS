```css
3D TRANSFORMATIONS

1. INTRODUCTION TO 3D TRANSFORMATIONS

  • 3D transformations affect elements along the X, Y, and Z axes.  
    Requires "perspective" to create depth.


2. TYPES OF 3D TRANSFORMATIONS

  • Perspective (Adds depth)  

    .perspective-container {  
        perspective: 500px;  
    }

  • Rotate3D (Rotates in 3D space)  

    .rotate3d-box {  
        width: 100px;  
        height: 100px;  
        background-color: mediumpurple;  
        transform: rotate3d(1, 1, 0, 45deg);  
    }

  • Translate3D (Moves in 3D space)  

    .translate3d-box {  
        width: 100px;  
        height: 100px;  
        background-color: tomato;  
        transform: translate3d(50px, 20px, 30px);  
    }

  • Scale3D (Resizes in 3D)  

    .scale3d-box {  
        width: 100px;  
        height: 100px;  
        background-color: darkcyan;  
        transform: scale3d(1.5, 1.5, 1);  
    }

  • Rotate X, Y, Z (Rotates along specific axes)  

    .rotate-x-box {  
        width: 100px;  
        height: 100px;  
        background-color: darkorange;  
        transform: rotateX(45deg);  
    }

    .rotate-y-box {  
        width: 100px;  
        height: 100px;  
        background-color: darkorchid;  
        transform: rotateY(45deg);  
    }

    .rotate-z-box {  
        width: 100px;  
        height: 100px;  
        background-color: darkslateblue;  
        transform: rotateZ(45deg);  
    }


3. EXTRA NOTES

  • Perspective works only on parent elements and affects child elements.  

  • 3D transformations work better when combined with animations.  


END OF NOTES
