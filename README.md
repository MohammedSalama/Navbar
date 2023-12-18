/**
 * Hides the modal window by adding the 'hide' class to the 'container' element and removing the 'hide' class from the 'btnOpen' element.
 */
btnClose.onclick = function() {
    container.classList.add('hide'); // adds the 'hide' class to the 'container' element
    this.classList.add('hide'); // adds the 'hide' class to the 'btnClose' element
    btnOpen.classList.remove('hide'); // removes the 'hide' class from the 'btnOpen' element
}

/**
 * Shows the modal window by removing the 'hide' class from the 'container' element and adding the 'hide' class to the 'btnClose' element.
 */
btnOpen.onclick = function() {
    this.classList.add('hide'); // adds the 'hide' class to the 'btnOpen' element
    btnClose.classList.remove('hide'); // removes the 'hide' class from the 'btnClose' element
    container.classList.remove('hide'); // removes the 'hide' class from the 'container' element
}

/**
 * Hides the modal window by adding the 'hide' class to the 'container' element and removing the 'hide' class from the 'btnClose' element.
 * @param {Event} event - The click event that triggered the function.
 */
btnClose.onclick = function(event) {
    container.classList.add('hide');
    btnClose.classList.remove('hide');
    btnOpen.classList.remove('hide');
}

/**
 * Shows the modal window by removing the 'hide' class from the 'container' element and adding the 'hide' class to the 'btnClose' element.
 * @param {Event} event - The click event that triggered the function.
 */
btnOpen.onclick = function(event) {
    btnClose.classList.remove('hide');
    btnOpen.classList.add('hide');
    container.classList.remove('hide');
}
