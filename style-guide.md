
#My styles.


*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    list-style: none;
}

:root {   
    --color-primary: #191d2b;
    --color-secondary: #27AE60;
    --color-white: #FFFFFF;
    --color-black: #000;
    --color-grey0: #f8f8f8;
    --color-grey-1: #dbe1e8;
    --color-grey-2: #b2becd;
    --color-grey-3: #6c7983;
    --color-grey-4: #454e56;
    --color-grey-5: #2a2e35;
    --color-grey-6: #12181b;
    --br-sm-2: 14px;
    --box-shadow-1: 0 3px 15px rgba(0,0,0,.3);
  }

  body {
    background-color: var(--color-primary);
    font-size: 1.1rem;
    color: var(--color-white);
  }

  a {
    text-decoration: none;
  }

  .container {
    margin: 40px 0;
    padding: 3rem 10rem;
  }

 .header_content {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  
 }

 .header_content .left_header {
    display: flex;
    align-items: center;
    position: relative;
 }



/*Independed components*/
.btn-con {
  display: flex;
  align-self: flex-start;
}

.main-btn {
  border-radius: 30px;
  color: inherit;
  font-weight: 600;
  position: relative;
  border: 1px solid var(--color-secondary);
  display: flex;
  align-self: flex-start;
  align-items: center;
  overflow: hidden;
}
.main-btn .btn-text {
  padding: 0 2rem;
}
.main-btn .btn-icon {
  background-color: var(--color-secondary);
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  padding: 1rem;
}
.main-btn::before {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  transform: translateX(100%);
  transition: all 0.4s ease-out;
  z-index: -1;
}
.main-btn:hover {
  transition: all 0.4s ease-out;
}
.main-btn:hover::before {
  width: 100%;
  height: 100%;
  background-color: var(--color-secondary);
  transform: translateX(0);
  transition: all 0.4s ease-out;
}

.main-title {
  text-align: center;
}
.main-title h2 {
  position: relative;
  text-transform: uppercase;
  font-size: 4rem;
  font-weight: 700;
}

 .controls {
    top: auto;
    bottom: 0;
    flex-direction: row;
    justify-content: center;
    left: 50%;
    transform: translateX(-50%);
    width: 100%;
    background-color: var(--color-grey-5);
  }
  .controls .control {
    margin: 1rem 0.3rem;
  }



@media screen and (max-width: 600px)
.controls {
    top: auto;
    bottom: 0;
    flex-direction: row;
    justify-content: center;
    left: 50%;
    transform: translateX(-50%);
    width: 100%;
    background-color: var(--color-grey-5);
}