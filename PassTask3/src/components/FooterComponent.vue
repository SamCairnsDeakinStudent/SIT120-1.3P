<script setup>

</script>

<template>
    <footer class="amazing-footer" style="font-family: Arial, Helvetica, sans-serif;">
        <div class="footer-content">
            <div class="footer-section">
                <h4>About Me</h4>
                <p>Deakin University Student currently studying his first year in a Bachelor of Information Technology</p>
            </div>
            <div class="footer-section">
                <h4>Quick Links</h4>
                <ul>
                    <li><RouterLink class="nav-link" to="/">Home</RouterLink></li>
                    <li><RouterLink class="nav-link" to="/about">About</RouterLink></li>
                    <li><RouterLink class="nav-link" to="/contact">Contact</RouterLink></li>
                </ul>
            </div>
            <div class="footer-section">
                <h4>Contact Info</h4>
                <p><i class="fas fa-map-marker-alt"></i>123 Street, City, Country</p>
                <p><i class="fas fa-phone"></i>0123 4567</p>
                <p><i class="fas fa-envelope"></i>Contact@email.com</p>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; Sam. All rights reserved.</p>
        </div>
    </footer>
</template>

