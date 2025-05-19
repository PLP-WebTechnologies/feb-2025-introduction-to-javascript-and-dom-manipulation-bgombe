function sayHI() {
    console.log("Hello, World!");
    console.log("Goodbye world");
}

function changeText() {
    const para = document.getElementById('dynamicText');
    para.textContent = 'The text content has been changed dynamically!';
}

function changeStyle() {
    const heading = document.getElementById('mainHeading');
    heading.style.color = 'red';
    heading.style.fontSize = '2.5em';
    heading.style.backgroundColor = 'yellow';
}

function toggleElement() {
    const container = document.getElementById('elementContainer');
    let existing = document.getElementById('dynamicElement');
    if (existing) {
        container.removeChild(existing);
    } else {
        const newElem = document.createElement('div');
        newElem.id = 'dynamicElement';
        newElem.textContent = 'This element was added dynamically!';
        newElem.style.padding = '10px';
        newElem.style.marginTop = '10px';
        newElem.style.border = '1px solid black';
        container.appendChild(newElem);
    }
}
