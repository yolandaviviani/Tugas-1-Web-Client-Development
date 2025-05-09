# Tugas-1-Web-Client-Development

Find the circumference, area, and diameter of a circle
<script>
function countcircle(){
    const radius = parseFloat(document.getElementById("radius").value);
    
    // Calculate values
    const diameter = 2 * radius;
    const area = Math.PI * radius * radius;
    const circumference = Math.PI * 2 * radius;
    
    // Display results
    document.getElementById("diameter-result").textContent = "Diameter: " + diameter;
    document.getElementById("area-result").textContent = "Area: " + area.toFixed(3);
    document.getElementById("circumference-result").textContent = "Circumference: " + circumference.toFixed(4);
}

Find the area of a triangle
<script>
function calculatedArea(){
    let base = parseFloat(document.getElementById("base").value);
    let height = parseFloat(document.getElementById("height").value);
    let area = (base*height) / 2;
    document.getElementById("result").innerHTML = "Area: " + area;
}     
</script>

Find the angle 
<script>
function calculatedangle(){
    let sideA = parseFloat(document.getElementById("sideA").value);
    let sideB = parseFloat(document.getElementById("sideB").value);
    let angle = 180 - sideA - sideB
    document.getElementById("result").innerHTML = "angle: " + angle;
}     
</script>

Find the date difference
<script>
        function x() {
            const firstdate = document.getElementById("firstdate").value;
            const seconddate = document.getElementById("seconddate").value;

            const startTimestamp = new Date(firstdate).getTime();
            const endTimestamp = new Date(seconddate).getTime();

            const difference = endTimestamp - startTimestamp;

            const differenceInDays = Math.round(difference / (1000 * 60 * 60 * 24));

            const daycountelement = document.getElementById('daycount');
            daycountelement.innerHTML = `The difference between the dates is ${differenceInDays} days.`;
        }
    </script>
Print the Initial name in capital
<script>
    const fullName = prompt("Enter your full name:");
    const nameArray = fullName.split(" ");
    let initials = "";
    for (let i = 0; i < nameArray.length; i++) {
      initials += nameArray[i].charAt(0).toUpperCase();
    }
    document.getElementById("initials").textContent = initials;
  </script>

  
  
