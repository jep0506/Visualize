
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
    <meta name="description" content="">
    <meta name="author" content="">
    <link rel="icon" href="../../favicon.ico">

    <title>Jumbotron Template for Bootstrap</title>
    
      <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
  </head>

  <body>
 
<div class="container"></div>
    <body>
      <h2>Could education be a casualty of the digital divide?</h2>
      <p> States that have a higher percentage of people who have no internet access have been found to be the states with lower qualities of education. The map below shows that New Mexico (47.4 %) and Mississippi (49.7 %) are the two states that have the most people without internet access. This correlates with state education quality scores released by Education Week for 2016, where these states are ranked as the 49th and 50th respectively out of 51 (including the District of Columbia). The only state that did worse was Nevada, who has 36.8% of people unable to connect to the internet at home. </p> 

      
      <iframe width="100%" height="520" frameborder="20" src="https://jep0506.cartodb.com/viz/468fd70a-0b0a-11e6-84a2-0e98b61680bf/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

<p> Former Professor of Education at Hofstra University, Dr. Timothy Smith believes that “states do not necessarily have poor education due to the lack of internet connection, however it is linked. Students have less of an ability to keep up with global standards when they can’t connect to the internet.” </p>

<div id="container" style="min-width: 310px; height: 400px; max-width: 800px; margin: 0 auto"></div>

<p>EdWeek also recently did a story on Calhoun County, which is claimed to have the “slowest internet in Mississippi.” According to the article, the schools in this district have given up on online tools and "buying the new digital technologies that are transforming schools elsewhere." Some students feel as if they are falling behind other schools in the country. Clemmie Jean Weddle told EdWeek, "I had those 15 pages, and they had the Internet at their fingertips."</p>

<p>In the situation of Calhoun County, an entire school district is on the wrong side of the digital divide. How about when you are the one of a few students at your school that can’t connect?</p>

<p>At Calhoun County schools, teachers and students knew there was an issue with connecting to the internet because they were all experiencing it. Therefore, teachers were straying away from using online tools and other technology that would create an issue for students to complete or have access to. Students that don’t have internet at home, while their peers do tend to fall behind in the classroom.</p>

<p>Rachel Monahan wrote an article for The Atlantic telling the story of the Kent School DIstrict who tried to bridge the digital divide by giving students their own laptops. However, some students weren’t bringing their laptops home because they couldn’t connect there. According to the Atlantic, about 2,500 students in Kent  cannot connect to the internet once they get home. When the laptops were given out, the curriculum moved toward “project- based learning” which heavily relies on the Internet. As Thuan Nguyen tell the Atlantic, “if you’re not able to provide that last level of connectivity, you’ve now widened the gap in terms of what kids can do, not to mention the expectation around that.” </p>

<p>Dr. Smith says that not having home Internet connection makes simple tasks a lot harder for students because they can’t do work at home. “It will take a lot more effort and a lot more time, and not everyone has the luxury of having these open for school work.” </p>

<p>These problems have not gone unnoticed by politicians and by President Obama who has started initiatives to try to make sure every school has access to the internet through a program called ConnectEd. He announced this initiative in June 2013, and vowed “that within the next 5 years, 99% percent of students would be connected to next- generation broadband and high- speed wireless in their school and libraries.” </p>

<p>	However Obama has not only focused on schools, the offshoot of ConnectEd, ConnectHome, plans to increase internet access for low income families. On the website, ConnectHome is described as a “public- private collaboration to narrow the digital divide for families with school- age children who live in HUD- assisted housing.” It is considered to be the next step in Obama’s vow to close the digital divide. </p>

<p>“This generation is claimed to have the whole world at its fingertips, however we have to account for the many that are left out,” said Dr. Smith. </p>
</body>

      <hr>

      <footer>
        <p>&copy; 2015 Company, Inc.</p>
      </footer>



    <!-- Bootstrap core JavaScript
    ================================================== -->
    <!-- Placed at the end of the document so the pages load faster -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
    <script>window.jQuery || document.write('<script src="../../assets/js/vendor/jquery.min.js"><\/script>')</script>
    <script src="../../dist/js/bootstrap.min.js"></script>
    <!-- IE10 viewport hack for Surface/desktop Windows 8 bug -->
    <script src="../../assets/js/ie10-viewport-bug-workaround.js"></script>
    <script src="https://code.highcharts.com/highcharts.js"></script>
<script src="https://code.highcharts.com/modules/exporting.js"></script>

<script>
$(function() {
  $('#container').highcharts({
    chart: {
      type: 'scatter',
      zoomType: 'xy'
    },
    title: {
      text: 'State Education Quality Score vs. State Internet Access'
    },
    subtitle: {
      text: 'Source: EdWeek 2016'
    },
    xAxis: {
      title: {
        enabled: true,
        text: 'State Education Quality'
      },
      startOnTick: true,
      endOnTick: true,
      showLastLabel: true
    },
    yAxis: {
      title: {
        text: 'People Without Internet Access (%)'
      }
    },
    legend: {
      layout: 'vertical',
      align: 'left',
      verticalAlign: 'top',
      x: 100,
      y: 70,
      floating: true,
      backgroundColor: (Highcharts.theme && Highcharts.theme.legendBackgroundColor) || '#FFFFFF',
      borderWidth: 1
    },
    plotOptions: {
      scatter: {
        marker: {
          radius: 5,
          states: {
            hover: {
              enabled: true,
              lineColor: 'rgb(100,100,100)'
            }
          }
        },
        states: {
          hover: {
            marker: {
              enabled: false
            }
          }
        },
        tooltip: {
          headerFormat: '<b>{series.name}</b><br>',
          pointFormat: '{point.x}, {point.y} %'
        }
      }
    },
    series: [{
      name: 'States',
      color: 'rgba(223, 83, 83, .5)',
      data: [
        [68.1, 42.8],
        [75.1, 31.7],
        [68.5, 36.5],
        [69.8, 45.3],
        [69.8, 37.6],
        [74.5, 27.3],
        [82.5, 27],
        [72.9, 36],
        [76.8, 34.9],
        [72.4, 33.9],
        [71.9, 36.6],
        [74, 39.4],
        [67.9, 32.1],
        [76.6, 35.4],
        [74.9, 38.4],
        [76.2, 33.7],
        [73.8, 30.6],
        [73.3, 39.8],
        [68.7, 40.4],
        [78.5, 31.2],
        [82.7, 30.6],
        [86.8, 29.6],
        [71.7, 31.2],
        [79.6, 25.4],
        [65.6, 49.7],
        [72.2, 38.4],
        [72.8, 41.7],
        [76.5, 32.5],
        [65.2, 36.8],
        [82.3, 24.1],
        [85.1, 30.6],
        [65.8, 47.4],
        [79.8, 35.1],
        [70.6, 38.5],
        [77.1, 34.4],
        [74.7, 36.2],
        [68.2, 41.8],
        [70.2, 30.2],
        [80.5, 36],
        [78.9, 32.4],
        [69.6, 41.3],
        [70.3, 34.2],
        [70.9, 43.3],
        [69.7, 43.7],
        [72.2, 29.2],
        [83.8, 30.1],
        [79.2, 34.8],
        [74.9, 24.6],
        [71.8, 40.9],
        [79.4, 29.4],
        [80.2, 31.8]
      ]
    }]
  });
});
</script>

