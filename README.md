# uc-template

# for footer use only to activate thankyou page for contact 7
# for all contact form
<script>
  document.addEventListener('wpcf7mailsent', function () {
    window.location.href = "https://urbanfeatconstruction.com/thank-you";
  }, false);
</script>
# for specific contact form
<script>
  document.addEventListener('wpcf7mailsent', function (event) {
    // Replace 123 with your actual form ID (optional)
    // or remove the condition to apply to all forms
    if (event.detail.contactFormId == 123) {
      window.location.href = "https://yourdomain.com/thank-you";
    }
  }, false);
</script>
