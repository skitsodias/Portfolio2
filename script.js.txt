document.addEventListener("DOMContentLoaded", function () {
  const form = document.querySelector("form");
  const confirmation = document.querySelector("#confirmation");

  form.addEventListener("submit", function (e) {
    e.preventDefault();
    form.style.opacity = 0;
    setTimeout(() => {
      form.style.display = "none";
      confirmation.style.display = "block";
      confirmation.style.opacity = 1;
    }, 500);
  });
});
