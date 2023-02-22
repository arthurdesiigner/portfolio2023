<script>
// DRAGGABLE INTERACTION
gsap.registerPlugin(Draggable);
let draggableTimeline;
let draggableItem = $(".box");
let draggableContainer = $(".box-contain");

// Create a draggable element and animation
function createDraggable() {
  var midPoint =
    draggableContainer.innerWidth() / 2 - draggableItem.innerWidth() / 2;
  var endPoint = draggableContainer.innerWidth() - draggableItem.innerWidth();

  // Sync the draggable item with the animation timeline
  function updateTimeline(draggableObject) {
    let myVar = draggableObject.x / draggableObject.maxX;
    draggableTimeline.progress(myVar);
  }

  // Create draggable item
  Draggable.create(draggableItem, {
    type: "x",
    bounds: draggableContainer,
    inertia: true,
    // onDrag
    onDrag: function (e) {
      updateTimeline(this);
    },
    onMove: function (e) {
      updateTimeline(this);
    },
    onThrowUpdate: function (e) {
      updateTimeline(this);
    },
    maxDuration: 0.4,
    snap: { x: [0, Math.round(midPoint), Math.round(endPoint)] }
  });

  // Create drag timeline animation
  draggableTimeline = gsap.timeline({
    paused: true,
    defaults: { ease: Linear.easeNone }
  });
  let myScale = 2;
  draggableTimeline.fromTo(
    ".box-inner",
    {
      duration: 1,
      scaleY: 1,
      scaleX: 1,
      borderRadius: "3em"
    },
    {
      duration: 1,
      scaleY: myScale,
      scaleX: myScale,
      borderRadius: "1em"
    }
  );
  draggableTimeline.fromTo(
    ".box-inner",
    {
      duration: 1,
      scaleY: myScale,
      scaleX: myScale,
      borderRadius: "1em"
    },
    {
      duration: 1,
      scaleY: 1,
      scaleX: 1,
      borderRadius: "3em"
    }
  );
  draggableTimeline.progress(1.5);
}

// Whenever the window is resized, restart draggable
let windowWidth = window.innerWidth;
$(window).resize(function () {
	if (windowWidth !== window.innerWidth) {
    windowWidth = window.innerWidth;
    draggableTimeline.kill();
    Draggable.get(".box").kill();
    draggableItem.css("transform", "translate(0)");
    createDraggable();
  }
});
createDraggable();

// SCROLL INTERACTION
let click = document.getElementById("click");
click.load();
gsap.registerPlugin(ScrollTrigger);

// On page load set image to first collection item image
$(".image").attr("src", $(".work_item").eq(0).find(".work_img").attr("src"));

// Anytime item is scrolled into view
function updateImages(currentItem) {
  $(".work_item").removeClass("active");
  currentItem.addClass("active");
  let imageSrc = currentItem.find(".work_img").attr("src");
  $(".image").attr("src", imageSrc);
  click.currentTime = 0;
  click.play();
}

// Scroll into view trigger
$(".work_item").each(function (index) {
  let triggerElement = $(this);
  let tl = gsap.timeline({
    scrollTrigger: {
      trigger: triggerElement,
      // trigger element - viewport
      start: "top center",
      end: "bottom center",
      onEnter: () => {
        updateImages(triggerElement);
      },
      onEnterBack: () => {
        updateImages(triggerElement);
      }
    }
  });
});
</script>
