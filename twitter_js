
let header = null 

function getHeader () {
    if (header !== null) {
        createButton()
        createButton2()
        return
    } else {
        header = document.querySelector('header')
        setTimeout(getHeader, 100)
    }
}

//adds button to show any time anyone I follow has typed "book" "amazon.com" or "goodreads.com" sorted by latest
function createButton () {
  const targetElement = document.querySelector('[data-testid="SideNav_NewTweet_Button"]')
  const buttonParent = targetElement.parentElement

  const newButton = document.createElement('div')
  // Make the content a SVG image
  newButton.innerHTML = `
    <img src="https://raw.githubusercontent.com/neilhacker/icons/main/book.png" width="28" height="28" />
    <input type="color" id="book-button" value="#000000" style="position: absolute; top: 0; left: 0; right: 0; bottom: 0; opacity: 0; width: 100%; height: 100%; cursor: pointer;" />  
  `
  // Add styling
  newButton.style = 'width: 100%; display: flex; justify-content: left; align-items: center; position: relative; margin-top: 0px; margin-left: 12px; cursor: pointer;'
  newButton.id = 'bookButton'
  buttonParent.appendChild(newButton)

  // Add event listener
  const bookBth = document.getElementById('book-button')
  bookBth.addEventListener('click', (event) => {
    window.location='https://twitter.com/search?q=(book%20OR%20amazon.com%20OR%20goodreads.com)&src=typed_query&f=live&pf=on';
  })
  console.log(newButton)
}

// adds button to take my to my list of climate people (private list)
function createButton2 () {
  const targetElement = document.querySelector('[data-testid="SideNav_NewTweet_Button"]')
  const buttonParent = targetElement.parentElement

  const newButton = document.createElement('div')
  // Make the content a SVG image
  newButton.innerHTML = `
    <img src="https://www.nicepng.com/png/full/283-2830068_environmental-services-leaf-icon-white-png.png" width="28" height="28" />
    <input type="color" id="climate-button" value="#000000" style="position: absolute; top: 0; left: 0; right: 0; bottom: 0; opacity: 0; width: 100%; height: 100%; cursor: pointer;" />  
  `
  // Add styling
  newButton.style = 'width: 100%; display: flex; justify-content: left; align-items: center; position: relative; margin-top: 35px; margin-left: 12px; cursor: pointer;'
  newButton.id = 'climateButton'
  buttonParent.appendChild(newButton)

  // Add event listener
  const climateBth = document.getElementById('climate-button')
  climateBth.addEventListener('click', (event) => {
    window.location='https://twitter.com/i/lists/1359604008432914434';
  })
  console.log(newButton)
}


getHeader()
