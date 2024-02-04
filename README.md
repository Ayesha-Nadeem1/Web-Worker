********---Web Worker Data Processing Application Readme---********

This is a web application that demonstrates the use of Web Workers for heavy data processing tasks. It includes HTML, JavaScript, and Web Worker scripts to showcase the performance difference between processing data with and without Web Workers.

****---Prerequisites---****

   -> Internet connection (to load the application and scripts)
   
   -> Web browser with Web Workers support

****---How to Use---****

   1. Clone or download the repository.
   
   2. Open the `index.html` file in a modern web browser.
   
   3. Click the "Start Processing" button to initiate data processing tasks.
   
   4. The application will display the time taken for data processing with and without Web Workers.

****---Customization---****

   -> Adjust Array Size:
      Modify the `generateRandomArray` function in the script to test with larger or smaller datasets.

****---Summary of Findings---****

   The application demonstrates a noticeable performance improvement when using Web Workers for heavy data processing. By offloading tasks to Web Workers, the main thread remains responsive, providing a smoother user experience. The performance gains are more evident with larger datasets, where parallel execution significantly reduces processing time.

****---Challenges and Solutions---****

   One challenge faced was the need to dynamically create a Web Worker script. This was overcome by generating the Web Worker script content within the main JavaScript file and creating a Blob object to serve as the Web Worker source.

   Additionally, managing the communication between the main thread and Web Workers required careful handling of data exchange. The use of the `postMessage` API facilitated this communication, ensuring seamless coordination between threads.

****---Resources---****

https://web.dev/articles/workers-basics

for the use of 'Inline Workers'
