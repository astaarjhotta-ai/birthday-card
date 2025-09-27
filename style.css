function playSurprise() {
  // Play music
  document.getElementById("song").play();

  // Show love message
  document.getElementById("surprise").innerHTML = "🎉💖 A Big Hug & Lots of Love for You 💖🎉";

  // Speed up balloons
  document.querySelectorAll('.balloon').forEach(balloon => {
    balloon.style.animationDuration = "4s";
  });

  // Confetti explosion 🎊
  launchConfetti();
}

function launchConfetti() {
  // Burst effect
  confetti({
    particleCount: 150,
    spread: 100,
    origin: { y: 0.6 }
  });

  // Continuous falling confetti for a few seconds
  let duration = 3 * 1000; // 3 seconds
  let end = Date.now() + duration;

  (function frame() {
    confetti({
      particleCount: 5,
      angle: 60,
      spread: 55,
      origin: { x: 0 }
    });
    confetti({
      particleCount: 5,
      angle: 120,
      spread: 55,
      origin: { x: 1 }
    });

    if (Date.now() < end) {
      requestAnimationFrame(frame);
    }
  }());
}
