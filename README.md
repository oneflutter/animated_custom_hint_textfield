<h2>custom_animated_hint_textfield</h2>
<p>The <strong>Custom Animated Hint TextField</strong> is a Flutter package that enhances text input fields with dynamic and visually appealing animations for hint texts. You can create unique animations like cyclic scrolling, sliding, scaling, fading, and more, while maintaining the flexibility to customize the design and behavior to suit your app’s needs.</p>

<h2>Examples:</h2>


<img src="https://github.com/user-attachments/assets/2c952678-3c0e-46a6-a068-02424aeacde2" alt="custom_animated_hint_textfield1" height="400" width="250">
<img src="https://github.com/user-attachments/assets/16d2bb09-48e6-4bcf-867c-0af5a657f36c" alt="animated_custom_hint_textfield_" height="400" width="250">
<img src="https://github.com/user-attachments/assets/92cb5af7-0bfc-40aa-9f61-52d234ac5126" alt="1" height="400" width="200">

<br>

<img src="https://github.com/user-attachments/assets/3e42ab56-a81d-4d97-b2aa-9ebccdef719e" alt="custom_animated_hint_textfield3" height="400" width="225">
<img src="https://github.com/user-attachments/assets/d8628a89-9a51-4562-9790-8a995a158bad" alt="custom_animated_hint_textfield4" height="400" width="225">
<img src="https://github.com/user-attachments/assets/bf141676-6c07-4a06-8855-57d4954704b2" alt="custom_animated_hint_textfield1" height="400" width="225">


<h2>Features</h2>
<ul>
  <li>
    <strong>Animated Hint Text</strong>: Effortlessly add dynamic animated hints to your text field by providing a list 
    (e.g., <code>["A", "B", "C", "D", "E"]</code>) to the <code>hints:</code> parameter, enabling seamless animations that change dynamically.
  </li>
  <li>
    <strong>Multiple Animation Types</strong>: Includes cyclic scrolling, slide, scale, fade, and other animation effects for your hint text.
  </li>
  <li>
    <strong>Customizable Design</strong>: Customize the hint text style, animation duration, and other properties to match your app's design.
  </li>
  <li>
    <strong>Static and Animated Hints</strong>: Support for both static and animated hint text transitions.
  </li>
  <li>
    <strong>Cross-Platform Compatibility</strong>: Fully supports <strong>iOS</strong>, <strong>Android</strong>, and <strong>web</strong> platforms.
  </li>
</ul>

<h2>Installation</h2>
<p>Add <code>custom_animated_hint_textfield</code> as a dependency in your <code>pubspec.yaml</code> file:</p>
<pre><code> 
dependencies:
  custom_animated_hint_textfield: ^latest_version
</code></pre>
<p>Then, run <code>flutter pub get</code> to fetch the package.</p>

<p>Then, import it in your Dart file:</p>
<pre><code> 
import 'package:custom_animated_hint_textfield/custom_animated_hint_textfield.dart';
</code></pre>

<h2>Usage 1: "CircularAnimatedHintTextField" </h2>
<p>The <strong>Custom Animated Hint TextField</strong> widget allows you to create a dynamic and visually appealing text input field with animated hints that guide the user. You can easily customize the hint text, animations, and styles to suit your app's design and functionality. Here's how you can use it:</p>

<pre><code>
CircularAnimatedHintTextField(
  // The prefix icon displayed on the left side of the text field. 
  // You can customize the icon and color to fit your design.
  prefixIcon: Icon(Icons.search_off_rounded, color: Colors.purple), 
  
  // The suffix icon displayed on the right side of the text field.
  // Similar to the prefix icon, you can change it based on your requirements.
  suffixIcon: Icon(Icons.access_time_filled, color: Colors.purple),

  // The static hint text that appears when the text field is empty.
  // This text can be customized to guide the user on what to input. 
  staticHintText: "Search food...",  // <-- Modify this to change the default hint text.
  
  // The style applied to the static hint text. 
  // This allows you to change the color, font size, and other text styling properties.
  staticHintTextStyle: TextStyle(color: Colors.grey, fontSize: 14),  // <-- Modify this for different text styles for the static hint.
  
  // A list of animated hint texts that will appear in sequence.
  // Customize these texts to provide more suggestions, like popular searches or categories.
  hints: [
    "Burger Delights 🍔",
    "Pizza Heaven 🍕",
    "Sweet Treats 🍰",
    "Noodles Galore 🍜",
    "Taco Time 🌯",
    "Fries Galore 🍟",
  ],
  
  // The style applied to the animated hint text.
  // This style is for the hint text shown when the user interacts with the text field.
  // Customize it for a bolder or different color/style for better visibility.
  animatedHintTextStyle: TextStyle(fontSize: 14, color: Colors.black, fontWeight: FontWeight.bold),
)
</code></pre>

<p>If you prefer not to use the static hint text, you can leave out the <code>staticHintText</code> and <code>staticHintTextStyle</code> properties. Only the animated hint text will be displayed, cycling through the values provided in the <code>hints</code> list.</p>

<h3>Example:</h3>
<pre><code>
CircularAnimatedHintTextField(
  // You can leave out static hint text if you don't want a default hint.
  // staticHintText: "Search food...",
  // staticHintTextStyle: const TextStyle(color: Colors.grey, fontSize: 14),
  prefixIcon: Icon(Icons.search_off_rounded, color: Colors.purple), 
  suffixIcon: Icon(Icons.access_time_filled, color: Colors.purple),
  hints: [
    "Spicy Dishes 🌶️",
    "Quick Meals 🍴",
    "Healthy Options 🥗",
    "Desserts 🍦",
    "Vegan Delights 🌱",
  ],
  animatedHintTextStyle: TextStyle(fontSize: 16, color: Colors.green, fontWeight: FontWeight.bold),
)
</code></pre>

<p>The animated hints will automatically cycle through the provided list of suggestions, providing a more dynamic search experience for your users.</p>

<img src="https://github.com/user-attachments/assets/42835fd5-187c-4ceb-9e10-d16805798b1c" alt="animated_field_A" height="400" width="230">
<img src="https://github.com/user-attachments/assets/92cb5af7-0bfc-40aa-9f61-52d234ac5126" alt="1" height="400" width="200">
<img src="https://github.com/user-attachments/assets/2433e58b-cf4a-49fc-81b7-03d62e34c856" alt="2" height="400" width="200">


<h3>Customization Options</h3>
<ul>
  <li><strong>prefixIcon</strong>: Customize the icon on the left of the text field.</li>
  <li><strong>suffixIcon</strong>: Customize the icon on the right of the text field.</li>
  <li><strong>staticHintText</strong>: Set a static default hint text.</li>
  <li><strong>staticHintTextStyle</strong>: Customize the style of the static hint text.</li>
  <li><strong>hints</strong>: Provide a list of animated hint texts to display sequentially.</li>
  <li><strong>animatedHintTextStyle</strong>: Set the style for the animated hint text that appears during user interaction.</li>
</ul>


<h2>Usage 2: "AnimatedHintTextField" </h2>

<h3>Type Of Animation:</h3>
<pre><code>
  hintAnimationType: HintAnimationType.fade,
  hintAnimationType: HintAnimationType.slide,
  hintAnimationType: HintAnimationType.scale,
  hintAnimationType: HintAnimationType.slideFromTop,
  hintAnimationType: HintAnimationType.slideFromBottom,
  hintAnimationType: HintAnimationType.topToBottom,
  hintAnimationType: HintAnimationType.bottomToTop,
</code></pre>

<p>Here is an example usage of the <strong>Custom Animated Hint TextField</strong> widget:</p>
<h2>Example [static text with animated hint]</h2>
<pre><code>
AnimatedHintTextField(
  animateHintText: false,
  staticHintText: "Search... ",
  staticHintTextStyle: const TextStyle(fontSize: 14, color: Colors.grey),
  hints: const [
    'Quick Search 💡',
    'Explore More 🌍',
    'Find Your Favorite 🔍',
  ],
  fieldBackgroundColor: Colors.grey[200],
  animatedHintTextStyle: const TextStyle(fontSize: 16, color: Colors.black),
  hintSwitchDuration: const Duration(seconds: 2),
  hintAnimationType: HintAnimationType.fade,
),
</code></pre>

<h3>Output:</h3>
<p>Image that showcasing the <strong>Custom Animated Hint TextField</strong> in action:</p>

<img src="https://github.com/user-attachments/assets/2c952678-3c0e-46a6-a068-02424aeacde2" alt="custom_animated_hint_textfield1" height="400" width="250">

<h2>Example [Animated hint without static Text]</h2>
<pre><code>
// Fade Animation
AnimatedHintTextField(
 // animateHintText: false,
 // staticHintText: "Search... ",
 // staticHintTextStyle: const TextStyle(fontSize: 14, color: Colors.grey),
 hints: const [
     'Quick Search 💡',
     'Explore More 🌍',
     'Find Your Favorite 🔍',
   ],
 fieldBackgroundColor: Colors.grey[200],
 animatedHintTextStyle: const TextStyle(
       fontSize: 15,
       color: Colors.black,
       fontWeight: FontWeight.bold),
 hintSwitchDuration: const Duration(seconds: 2),
 hintAnimationType: HintAnimationType.fade,
)
</code></pre>

<h2>Output:</h2>
<p>Image that showcasing the <strong>Custom Animated Hint TextField</strong> in action:</p>
<img src="https://github.com/user-attachments/assets/16d2bb09-48e6-4bcf-867c-0af5a657f36c" alt="animated_custom_hint_textfield_" height="400" width="250">


<h2>Animation Types</h2>
<ul>
  <li><strong>Cyclic Scrolling</strong>: The hint text scrolls cyclically, looping through the provided hints. [use CircularAnimatedHintTextField widget]</li>
  <li><strong>Slide Animation</strong>: Hints slide in and out of the text field horizontally. [use AnimatedHintTextField widget]</li>
  <li><strong>Scale Animation</strong>: The hint text scales in and out for a zoom effect. [use AnimatedHintTextField widget]</li>
  <li><strong>Fade Animation</strong>: Hints fade in and out for a smooth transition effect. [use AnimatedHintTextField widget]</li>
  <li><strong>Vertical Animations</strong>: Hints move vertically (top-to-bottom or bottom-to-top) through the text field. [use AnimatedHintTextField widget]</li>
</ul>

<h2>Customization</h2>
<p>The package offers several properties for customization:</p>
<ul>
  <li><strong>Hint Style</strong>: Customize the static and animated hint text styles using <code>hintStyleForStatic</code> and <code>hintStyleForAnimatedHint</code>.</li>
  <li><strong>Icons</strong>: Add <code>prefixIcon</code> and <code>suffixIcon</code> for additional functionality or aesthetics.</li>
  <li><strong>Hint Transition Duration</strong>: Adjust the transition duration of hint text with <code>hintChangeDuration</code>.</li>
  <li><strong>Auto Focus</strong>: Automatically focus the input field when initialized.</li>
  <li><strong>Background Color</strong>: Set the background color of the text field.</li>
</ul>


<h2>Conclusion</h2>
<p>The <strong>Custom Animated Hint TextField</strong> package allows you to add beautiful and dynamic hint text animations to your Flutter applications, creating an engaging user experience. With multiple animation types and full customization options, you can tailor the animations to suit your app’s style.</p>

<h2>Feedback</h2>
<p>If you encounter any issues or have suggestions, feel free to contribute or open an issue on the GitHub repository. Your feedback is highly appreciated!</p>

