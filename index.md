---
layout: master
title: Index
---

<div class="container mt-5">
    <div class="row">
        <!-- Image on the Left -->
        <div class="col-lg-6">
            <img src="https://i.pinimg.com/originals/58/db/86/58db86530c4ed7af2cc2408d19542dec.png" class="img-fluid" alt="Large Image">
        </div>

        <!-- Information on the Right -->
        <div class="col-lg-6">
            <div class="container">
                <div id="typing-container"></div>

                <script>
                    document.addEventListener('DOMContentLoaded', function() {
                        var text = "Hello, my name is Greg Kohler";
                        var container = document.getElementById('typing-container');
            
                        function typeText(index) {
                            if(index < text.length) {
                                container.innerHTML += text.charAt(index);
                                index++;
                                setTimeout(function() { typeText(index) }, 100); // Adjust the timeout to control typing speed
                            } else {
                    // Show the body text once typing is finished
                                var bodyText = document.getElementById('body-text');
                                bodyText.style.display = 'block';
                            }
                        }
            
                        typeText(0);
                    });
                </script>
                <div id="body-text">
                I am a student at the University of Minnesota studying for my Masters in Geographic Information Sciences.
                </div>
            </div>
        </div>
    </div>
</div>

