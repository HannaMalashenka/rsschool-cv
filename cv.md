# Hanna Malashenka
## Contact Info
![Location](https://img.icons8.com/android/48/000000/worldwide-location.png) Minsk, Belarus

![Mobile Phone](https://img.icons8.com/fluent-systems-regular/48/000000/phone.png) +37529 377 76 75

[![Linkedin](https://img.icons8.com/fluent/48/000000/linkedin.png) Hanna Malashenka](https://www.linkedin.com/in/hanna-malashenka/)

[![GitHub](https://img.icons8.com/fluent/48/000000/github.png) hannamalashenka](https://github.com/HannaMalashenka)
## About
A specialist with versatile experience, 5 years in IT industry in QA sphere:
* Manual testing of a complex buisness solutions (Ad Platform, Cloud Data Migration, Tax app, etc);
* Automated testing for API and Web app (end-to-end) - C#, Java, Selenium, NUnit, Specflow, etc;
* QA Team management (4 engineers);
* Launched internal cources 'Networks for QA' for company trainees;
* Landing pages creation for company events and Marketing department needs (Wordpress, HTML, CSS, JS, PHP);
* Sales assistance in Pre-Sales department;
* Won 'Universal Player' nomination last year.

I always aim to self-develop, be a so called T-shaped specialist. Right now my goal is to skill up in front-end development and choose grouth vector for the next couple of years. 

## Skills
**Languages**: C#, Java, SQL, HTML, JS, PHP;

**Tools**: Postman, Fiddler, Swagger, Putty, Git, AWS, VirtualBox;

**Task-tracking**: Jira, Rally, Trello;

**CI/CD**: TFS, Azure, Jenkins.

## Code examples

```Java

/**
 * Exercise 3: Sort the product list
 *
 * Requirement
 *      * Sort product list by 'product name' in reverse alphabetical order
 *      * Exclude all 'null' product names
 *      * Print out the sorted list (you can call product.toString())
 */
@Test
	public void solution3() {
	    products.stream()
	            .filter(product -> product.getName()!= null)
	            .sorted(Comparator.comparing(Product::getPrice).reversed())
	            .forEach(System.out::println);
}
```

```javascript

function formv3(){
    var xhr = new XMLHttpRequest();
    var url = 'https://api.hsforms.com/submissions/v3/integration/submit/hubNumber/formNumber';
   
    var data = {
      "submittedAt": $.now(),
      "fields": [
        {
          "name": "firstname",
          "value": $('input[name="name"]').val()
        },
        {
          "name": "company",
          "value": $('input[name="company"]').val()
        },
        {
          "name": "email",
          "value": $('input[name="email"]').val()
        },
        {
          "name": "product_name",
          "value": $('input[name="product"]').val()
        },
        {
          "name": "qa_specialists_ballpark_estimates",
          "value": $('select[name="ballpark"]').val()
        },
        {
          "name": "your_software_product_overview",
          "value": $('input[name="overview"]').val()
        }
      ],
      "context": {
        "pageUri": window.location.href,
        "pageName": document.title
      },
      "legalConsentOptions":{
        "consent":{
          "consentToProcess": $("#gdpr").val(),
          "text": $('.legal-data-text').text(),
          "communications":[
            {
              "value": $("#communication").val(),
              "subscriptionTypeId": subscriptionNumber,
              "text": $('.legal-com-text').text()
            }
          ]
        }
      }
    }

    var final_data = JSON.stringify(data)

    xhr.open('POST', url);
    xhr.setRequestHeader('Content-Type', 'application/json');

    xhr.onreadystatechange = function() {
        if(xhr.readyState == 4 && xhr.status == 200) { 
            $('#form-msg').append('Thank you for filling out your information. Our expert will be back to you in the shortest possible time to discuss the details.');
        	clearFields();
        } else if (xhr.readyState == 4 && xhr.status == 400){ 
            $('#error').html('It looks like something went wrong. Please check the submitted data once again.');          
        } else if (xhr.readyState == 4 && xhr.status == 403){ 
            alert(xhr.responseText); // Returns a 403 error  submissions.           
        } else if (xhr.readyState == 4 && xhr.status == 404){ 
            alert(xhr.responseText); //Returns a 404 error if the formGuid isn't found     
        }
       }   
    xhr.send(final_data)
 }

```

```PHP

<?php
	$name=$_POST['name'];
	$company=$_POST['company'];
	$product=$_POST['product'];
	$email=$_POST['email'];

	$ballpark=$_POST['ballpark'];
	$overview=$_POST['overview'];
	$qa_challenge=$_POST['qa_challenge'];

	$qa_team=$_POST['qa_team'];
	$toolkit=$_POST['toolkit'];
	$comment=$_POST['comment'];

	$gdpr=$_POST['gdpr'];

	$emailTo = 'someemail@test.mail'; 
	$body = "Name: $name \n\nCompany: $company \n\nProduct name: $product \n\nEmail: $email \n\nQA specialists’ ballpark estimates: $ballpark \n\nYour software product overview: $overview \n\nQA challenges to focus on: $qa_challenge \n\nIn-house QA team: $qa_team \n\nProgramming language and toolkit: $toolkit \n\nComment: $comment \n\nGDPR: $gdpr \n\n";
	$subject = 'Test automation free POC';
	$headers = "From: Test automation free POC Landing Page <mail@mail.com> \r\nContent-type: text/plain; charset=utf-8 \r\n";

   if(mail($emailTo, $subject, $body, $headers)){
	   echo "<span>Thank you for filling out your information. Our expert will be back to you in the shortest possible time to discuss the details.</span>";
	} else {
		echo "<span>Woops, something goes wrong, please check your data.</span>";	
	};		
?>

```

## Education
__University:__  
Belarusian State University, FAMCS  
_Bachelor's degree_ 2013-2017

__Cources and Certificates:__
* SAFe Practitioner Certification
* SQL Advanced
* Life & Time management 
* Training for Trainers
* Business English

## Languages
__English__: B2
