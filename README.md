# T1A1-Workbook

## **Q1** Identify and explain common and important components and concepts of web development markup languages
### A markup language uses tags to define elements within a document. These languages contain standard words rather than typical programming syntax, making it easier for humans to understand.  I will be using examples from HTML to explain the important concepts and components of markup languages. In HTML, elements, tags and attributes are used to create structure within a document by defining sections, paragraphs and links. 

### Markup languages allow us to provide accessibility and support across a variety of browsers. For example I might have a hero image that works as expected on chrome but breaks on firefox, instead of leaving the user confused as to why it’s not displaying I can provide them with alt text that describes the image. Another example is keyboard accessibility, some users may want to navigate a page using different keys. HTML has built-in keyboard accessibility that allows the user to do just that. 

---

## **Q2** Define the features of the following technologies that are essential in terms of the development of the internet
**Packets**
Packets are small bits of data that are sent over a network, they can be sent via the internet or LAN (local area network). In order to reach their destination each packet includes a source and destination as well as the data being transferred. Packets travel via routers and routers choose the cheapest path for each piece of data, based on the destination. TCP is responsible for the sending and receiving of data as packets. The exact structure of packets varies between protocols, a typical packet includes two sections, a header and payload. Information about the packet is stored in the header and the actual data itself is stored in the payload. 

### The idea of packet switching was first studied by Len Kleinrock at MIT. While researching message switching his studies then became applicable to packet switching. After came the research of digitising and packetizing of important voice messages in the case of a nuclear attack. They envisioned a highly resilient voice network for command and control (1962).

### **IP Addresses**
### Every device connected to the internet is assigned a unique IP address. IPV4 addresses are 32 bits in length, written as four sets of numbers between 0 and 255, separated by dots. IP addresses are separated into two parts, the first part represents the network and the second part represents the host. When this was first introduced the idea was to make address allocation scaleable, they were split into 5 classes (A,B,C,D,E). The main classes used are A, B and C. D classes are called multicast addresses and E classes are reserved for experimental use. 

### The issue with IPv4 is there are not enough addresses left, Vint Cerf explained why the internet protocol v 4 ended up at 32-bits; “and we said how many countries are there? And we didn’t know the answer to that, and there wasn’t any Google to find out! So we guessed at 128. So two times 128 is 256 which takes 8 bits to represent which network you’re on. Then we said how many computers per network?”. The team eventually decided on 16 million computers per network which meant 24 bits were required for the host address.

### IPv6 is the latest version of the internet protocol, it will use 128-bit addressing to support almost 340 trillion devices. IPv6 will use eight groups of four hexadecimal digits. It will be able to support packets more efficiently and will improve performance and security. 

### **Routers**
### Routers allow us to connect computers and other devices to the internet. They decide the best route for your information to travel and protect our information from security threats. A router is connected to two or more data lines from different IP addresses, when a packet is received from another network the router reads the network information in the packet header to determine its destination. 

### Routers can exchange information about destination addresses by using a routing protocol. A router table is a data table stored inside a router or a network host, it is used to store route information about directly connected and remote networks. The software used to control the router is made up of two planes that operate simultaneously. The first part is a control plane; routes are stored in the routing table, the control plane builds a forwarding information base to be used by the forwarding plane. A forwarding plane forwards packets by reading the packet header of every packet it receives, it then finds the destination supplied by the control plane and directs the packets to the correct destination.

### **Domains and DNS**
### The rapid increase of computers on the network made it difficult to keep track of all the different IP addresses. The problem was solved by the introduction of DNS, which converted IP addresses into simple names that are easily read by humans.

### A domain name and its matching IP address is called a DNS record. Name servers are a type of server that keeps all the DNS records of your domain name, its job is to provide DNS information to anyone requesting it. Each domain name must have at least two name servers, the first being the primary server, if the first server doesn’t respond the secondary server is used to resolve the domain name. 

### The DNS process ensures things run quickly and smoothly. First, the initial request for the IP address is made. The search then leads to a root server, root servers are located all around the world and it will usually direct users to the closest one geographically. Once the request is made it then goes to the name server, which stores information about the site and its IP. Once this process is complete, it is sent back to the client and the user can now visit the website. This process is completed in milliseconds.

---

## **Q3** Define the features of the following technologies that are essential in terms of the development of the internet

### **TCP**
### TCP is the protocol on which the internet is built, it is a connection-oriented protocol and allows a device to send a packet to another device on the same network or on a different network. First, it establishes a connection with the receiver and attempts to send the packet. If the packet is unable to be sent it tries to resend the packet, the connection will not close unless the packet has been delivered or if an error occurs. TCP is always used for one-on-one communication, it cannot be used to broadcast messages.

### **HTTP aand HTTPS**
### HTTP is an application layer network protocol which is built on top of TCP.  It provides a standard set of rules to govern how information can be transmitted over the web. HTTP uses Hypertext structured text which establishes the link between nodes containing text. HTTP lacks many security features and the ability to encrypt data, for ecommerce sites or other sites that require sensitive data such as credit card numbers, HTTPS should be used. HTTPS is a highly secure version of HTTP, it is recognised and trusted by many users as it confirms a stable and secure connection and encrypted data. Although HTTPS is considered a reliable way to make transactions online there is no definite way to stop people from stealing confidential information on the browser, SSL data can only be encrypted during transmission so it can’t clear the text in the browser memory. 


### **TCP**
### A browser is a program that retrieves and displays pages from the web. Information in the browser is transferred using Hypertext transfer protocol, after this data is sent a rendering engine translates that data into text and images.Modern web browsers such as; Chrome, Firefox, Safari and Opera contain a suite of dev tools. These tools are used throughout the development process for testing, debugging and testing quick html changes. These tools can be accessed through shortcuts and features vary depending on the browser. There are many tools available within the Chrome browser some common examples include:
### - Mobile simulation: useful for testing layouts on  smaller screen sizes and the overall mobile experience
### - Debugging: the console log is useful for debugging when an unexpected error appears, this is useful on team projects to determine whether the issue was caused on the front-end or back-end 

---

## **Q4** Identify THREE data structures used in the Ruby programming language and explain the reasons for using each

### **Arrays**
### Arrays are an important data structure that can hold zero or many items, there are many useful methods that can be used to add, access and loop over these items. They can hold many different data types and are useful for condensing and organising code, making it more readable and maintainable. 

### **Hashes**
### Hashes are similar to arrays except their indexing is done via arbitrary keys rather than an integer index. In Ruby, a hash converts your key into a number by using the hash method. In this data structure every value has a key, which can be anything, such as a string or symbol.

### **Stacks**
### A stack is a data structure that processes elements by taking elements from the stack until it’s empty. A common example of stacks is to use them to flatten an array, stacks will push the elements inside the array back into the stack. If all elements are removed we are left with a flattened array. Ruby has the flatten method which does the same thing however it’s useful to understand how stacks work. 

---

## **Q5** Describe the features of interpreters and compilers and how they are different

### Computer programs are written using a high-level language, this is the source code of our programs. Computers cannot understand high-level; languages, it only undertones programs written in binary called the machine code. To convert source code into machine code we can use either a compiler or interpreter. Compilers scan the entire program and translate it as a whole. This process takes a large amount of time, however the overall execution time is faster compared to an interpreter. The main drawback to compiled code is its incapacity to be cross-platform, for example applications written on an Ubuntu machine cannot be installed on a windows machine. Interpreters take less time to analyse source code but the execution time is comparatively slower than compilers. Programming languages such as; JavaScript, Python and Ruby use interpreters. Interpreters are platform agnostic which means they can be run on any environment. The disadvantage of using interpreted codes is slower performance. 

---

## **Q6** Identify TWO commonly used programming languages and explain the benefits and drawbacks of each.

### **Ruby**
### The Ruby programming language is time efficient especially when it’s used in conjunction with the rails framework and allows you to develop things quickly. Another benefit to the language is the large and established community, although it has seen a decrease in popularity since 2019 as most programmers choose to develop using Java or Python. Ruby is considered to be very secure because of the built in security that looks for attacks. A downside to the language is the difficulty of implementing non-standard features, it can take a bit of time to customise configuration settings.



### **JavaScript**
### Javascript is simple to understand and easier to learn in comparison to other languages. It’s very popular and used by large companies such as Google, Amazon and Paypal. Another benefit of using Javascript is client-side validation, validation is possible on the browser itself rather than sending it off to the server . The number of built in features means that the performance of websites and applications is improved because of the reduced code length On the other-hand, since the code is visible to the user it may be used for malicious intent. Also the browser doesn’t show any errors making it harder to debug and locate issues. A single error can stop the rendering of the entire site, although browsers are tolerant of these errors. 

---

## **Q7** Case study

### **Topic 1:** access to a user’s personal information (medical, family, financial, personal attributes such as sexuality, religion, or beliefs)

### The collection of personal information and data happens quickly on the internet, data breaches are not uncommon and can directly affect customers and users. It is an IT professionals duty to be well versed in the various definitions and forms of privacy and should understand their rights and responsibilities associated with the collection and use of personal information. 

### Professionals should aim to collect the minimum amount of personal information necessary, users should be informed about where their data is stored and how long it is stored for. All users should consent to their information being collected. Data merging is the process of combining two or more data sets into a single data set, this process can compromise privacy features, therefore special care and consideration should be taken by the individual when merging collections. 

### As mentioned, data breaches can happen and the repercussions can cause a lot of harm for the users involved. Security should be a primary focus when designing and implementing systems. IT professionals should ensure that personal information is secure against accidental or intentional misuse of this information. If breaches occur it is the professionals responsibility to inform affected users in a timely manner and provide guidance and assistance to resolve the situation. 


## **Topic 2:** aggressive sales and marketing practices designed to mislead and deceive consumers

### According to the advertising and selling guide, published by the ACCC, it is illegal for a business to promote a product or service that is likely to mislead or deceive a consumer or other businesses. It is an IT professionals duty to flag any misleading or inaccurate information regarding a product or service with their manager. While the decision may not come from the professional directly, they should advocate for disclosing factual information about a product or service that is likely to change a customer's mind about purchasing a product or using a service.

### For example, a company offered ‘unlimited’ download plans for users who signed up to their service. However, the plans had major limitations such as speed reduction when a certain amount of data was downloaded. The federal court later fined the company due to misleading information as they did not disclose the plans limitations. While it’s not the professionals responsibility to market their product, the situation could have been avoided if the professional voiced their concerns about the misleading information. 



### Case Study: (https://catalyst.harvard.edu/wp-content/uploads/regulatory/ResearchDataLossIncidentCaseStudy.pdf) 

### The case study I have chosen focuses on data sharing between facilities and the use of personal information, particularly medical information of an individual. In the case study, a medical resident takes holiday leave, leaving his laptop at his medical office. It is worth noting that the resident travels frequently between medical practices where data sharing between the two practices occurs. While the resident is on leave, several offices are burglarised and the computer goes missing. The resident swears he encrypted his computer. 

### First, all affected individuals should be notified about the incident in a timely manner. The case study mentions that all data that’s been shared has been encrypted and this should be communicated to the individuals for their peace of mind. If any individuals request to have their stored information deleted, an IT professional should respond to this request immediately with confirmation of the deleted data. 

### Finally, the IT professional should comply and be well versed in the national data protection or privacy laws. They should ensure that no information is outsourced to third parties unless they also comply with these standards. The professional should review their companies security and regular patches should be made to the system to prevent unethical breaches.

---

## **Q8** Explain control flow, using examples from the Ruby programming language

### Control flow is the order in which a computer executes statements in a program. The code will run in order from the first statement to the last unless structures such as conditionals and loops, which change the flow of the program, are added. 

### Example code (https://zetcode.com/lang/rubytutorial/flowcontrol/) 

`num = gets.to_i

if num > 0 then

    puts "num variable is positive"
    puts "num variable equals to #{num}"
end`

### The ‘if’ keyword checks if an expression is true. The code above checks if the number inputted is greater than zero, if this condition is true two statements will print to the console. If the condition is false, nothing is printed. 

### The example above is quite simple and our programs will often have more complex problems to solve.

### The ‘else’ keyword is used to check if an expression evaluates to false. In both examples the block of code is enclosed with the ‘end’ keyword. The > operator checks if the value of the left operand is greater than the value on the right. If the condition is met this becomes true and the statement is printed to the console. If the condition is not met the second line is executed and the next statement is printed instead. 

### Example code (2) (https://zetcode.com/lang/rubytutorial/flowcontrol/) 

`age = 17

if age > 18

    puts "Driving license issued"
else

    puts "Driving license not permitted"
end`

---

## **Q9** Explain type coercion
### Type coercion is the conversion of values from one data type to another. There are two types of conversion, implicit and explicit. Type coercion is implicit, and type conversion is explicit. Explicit coercion is done by using inbuilt functions such as number(), string() and boolean(). 

### Implicit conversion does not require special syntax in the source code. For example, the Javascript engine will automatically convert data types, such as; string numbers and booleans, into their desired type. In boolean coercion, true values are equal to 1 and false values are equal to 0. When JavaScript notices the wrong data type it will automatically convert the value into the correct data type.

## **Q10** Explain data types, using examples

### Data types tell the computer how to handle the data in our program and determine what operations we can perform within our program. I will be using examples from Ruby to further explain data types. In Ruby all data types are based on classes because it is an object-oriented language. 

### The different types are as follows;
### - Arrays
### - Strings
### - Boolean
### - Hashes
### - Symbols
### - Numbers

### I will be giving examples from the first two data types. 

### Example code (1) (https://www.tutorialspoint.com/ruby/ruby_arrays.htm) 

### Arrays can hold many objects such as strings, hashes, symbols and can hold other array objects. We can initialise an array by using the ‘new’ class method. Arrays are useful for adding, accessing or looping over items easily. Some built-in class methods include; sort (used to sort strings or numbers inside an array), sample (used to pick one random element from an array), take (used to take the first 3 elements from an array). 

### Example code (2) (https://www.rubyguides.com/2018/01/ruby-string-methods/)   

### Strings are a sequence of characters. In its simplest form, strings are literals enclosed by single quotes. The code above extracts the substring, this is useful if we want to use a specific part of our string. The first number is the starting index and the second number is the length of characters to be extracted. 

--- 

## **Q11** Resturant classes


### Customer
### The first class I would create would be the customer class. We would need to store the customers data such as their name, email and address for delivery. I would assume the customer would need to sign up to the app first and their data would need to be stored for future orders. 

### Menu
### The next step would be creating the menu class. Menu items need a corresponding price and a short description of the item. The customer should be able to order the same item multiple times, they should be able to remove menu items from their order as well. 


### Order
### The customer information and order details would be stored in the order class. I am assuming that the restaurant would be pick-up only so there would need to be a corresponding order ID for when the customer reaches the restaurant. 

---

## **Q12** Identify and explain the error in the code snippet below that is preventing correct execution of the program:

### The error found in the code is a no method error.

### In order to multiply strings by other strings in Ruby we first need to convert the values into integers. The code will not function properly until the ‘Celsius’ and ‘Farenheit’ objects are converted using the to_i method. 

--- 
