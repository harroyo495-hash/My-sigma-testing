# My-sigma-testing
Day 1 
Hey poo poo head
from you but 1/31
Rainbow pen


let hueValue = 0;

function setup() {
  createCanvas(windowWidth, windowHeight);
  colorMode(HSL, 360); // Use HSL for easy rainbow colors
  background(255);
}

function draw() {
  // Rainbow color changes over time
  if (mouseIsPressed) {
    stroke(hueValue, 360, 200);
    strokeWeight(10);
    line(mouseX, mouseY, pmouseX, pmouseY);
    
    // Cycle hue
    hueValue += 2;
    if (hueValue > 360) {
      hueValue = 0;
    }
  }
}

// Optionally, change color on click
function mousePressed() {
  // Example: Change color immediately on click
  // hueValue = random(360);
}
