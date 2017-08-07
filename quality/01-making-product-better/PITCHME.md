## Making products easy to test
#### Karel Piwko, Red Hat Inc.
#### Aug 2017 
---

#### Part of Quality Engineer Responsibilities in Agile Series

Note: 
This series is aimed at both quality engineers familiar their job responsibilities within Waterfall model to facilitate their transition to Agile workflows
as well as for people from other teams, such as engineering that start to focus on quality aspects of the product as part of their daily job responsibilities.
 
---

**What is testing?**
* Finding Defects
* Gaining Confidence about Product Quality
* Providing Information for Decision Making
* Preventing Defects

<span style="float: right; font-style: italic">- ISTQB Syllabus, chapter 1</span>

Note:  
All are valid for for Agile workflow as well. The important thing to consider here is that a defect (bug, fault) can be not only in code but also in documentation, user story, requirements or acceptance criteria. The biggest benefit of Agile workflow is ability to aim on different quality related activities during team cooperation. This is sometimes referred to as iterative-incremental model and it is solely up the team to establish what is an interation (for Scrum, for instance an interation would likely map to a sprint) and what scope of testing activities should be executed at each iteration.

---

**Usual Feature lifecycle**
* Customer requirement
* Business evaluation for TCO, ROI
* Research, feature specification and planning
* Development, verification and validation
* Regression tests
* Deployment to production
* Maintenance

<span style="float: right; font-style: italic">Each could happen multiple times in an iteration</span>

Note:
TCO means Total Costs of Ownership, ROI means Return on Investement. Verification means "Am I building the product right?" whereas validation means "Am I building the right product?". As an example, usual testing activities, such as integration or end to end testing would be a part of validation phase whereas use stories review would be rather verification. Regression testing can be executed in multiple environments, such as in simplified CI [Continuous Integration] or in production like environment. Usually, a new feature development should for a regression test plan for future releases/iterations or even better, lead to automation of test scenarios so they do not regress in future. A decision what to automate a test scenario or not should be made together with ROI and TCO for its automation.

---

Let's talk about how you make product easy to test knowing what is testing and what is usual feature lifecycle

Note:
Spoiler alert: Quality focused work can make product easier to test in every phase of the lifecycle. It works the best though if implemented from the very begginning as sooner feedback/action is available, the cheaper is to put any resulting changes into action. On the next slide, there will be chart showing cost ration and various stages of product development.

---

Impact of making changes

<canvas data-chart="line">
<!-- 
{
  "data": {
    "labels": [1,2,3,4,5,6,7,8,9,10,11,12,13],   
    "datasets": [{
      "data": [4,4,6,8,12,16,20,26,32,48,64,96,128],
      "fill": "start",
      "cubicInterpolationMode": "monotone",
      "pointRadius": 0  
    }]
  },  
  "options": { 
    "responsive": "true",
    "title": {
      "display": "true",
      "text": "Change costs",
      "fontSize": 36
    },
    "legend": {
      "display": false
    },
    "scales": {
      "xAxes": [{
        "ticks": {
          "display": false
        },
        "scaleLabel": {
          "display": true,
          "labelString": "Time →",
          "fontSize": 36
        },
        "gridLines": {
          "display": false
        }
      }],
      "yAxes": [{
        "ticks": {
          "display": false
        },
        "scaleLabel": {
          "display": true,
          "labelString": "Effort →",
          "fontSize": 36
        },
        "gridLines": {
          "display": false
        }
      }]
    }    
  }
};
-->
</canvas>

Note:
It actually depends on product itself how the actual chart looks like but there are multiple elements to consider with respect to any such change and the costs. Products based on pluggable architectures or standalone services are usually less vulnerable to changes - but still the costs could be very high. As Agile workflows support and welcome changes, especially the ones based on customer feedback, it is crutial to incorporate feedback at low left corner.

---

## Customer requirements

+++

foo


