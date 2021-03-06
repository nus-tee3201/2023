{% from "common/macros.njk" import get_date with context %}

{% set weekly_ip_tasks = {
week2: [
  {id: 'learn_about_the_project'},
  {id: 'set_up_prerequisites'},
  {id: 'set_up_project'},
  {id: 'add_increments', suffix: ' (+ commit, tag, push)', deadline: 'before next lecture', increments: [
    {id: 'Level-0', title: 'Greet'},
    {id: 'Level-1', title: 'Greet, Echo, Exit'},
    {id: 'Level-2', title: 'Add, List'},
    {id: 'Level-3', title: 'Mark as Done'}
  ]}
],
week3: [
  {id: 'finish_leftover_tasks'},
  {id: 'create_pr_to_upstream', deadline: 'by the end of the lecture'},
  {id: 'add_increments', suffix: '', increments: [
    {id: 'Level-4', title: 'ToDo, Event, Deadline'},
    {id: 'A-TextUiTesting', title: 'Automated Text UI Testing', tag: 'optional'},
    {id: 'A-CodingStandard', title: 'Follow the Coding Standard'}
  ]}
],
week4: [
  {id: 'add_increments', suffix: ' as branches', increments: [
    {id: 'Level-5', title: 'Handle Errors'},
    {id: 'A-CodeQuality', title: 'Improve Code Quality'},
    {id: 'A-AbstractClasses', title: 'Use Abstract Classes'},
    {id: 'A-Packages', title: 'Organize into Packages'}
  ]},
  {id: 'use_gfmd_in_pr_description'},
  {id: 'review_two_prs', graded: true}
],
week5: [
  {id: 'add_increments', suffix: ' as PR', increments:  [
    {id: 'Level-6', title: 'Delete'}
  ]},
  {id: 'add_increments', suffix: ' as parallel branches', increments:  [
    {id: 'Level-7', title: 'Save'},
    {id: 'A-JavaDoc', title: 'JavaDoc'}
  ]},
  {id: 'add_increments', suffix: '', increments:  [
    {id: 'A-Jar', title: 'Create a JAR File'}
  ]}
],
week6: [
  {id: 'add_increments', suffix: '', increments:  [
    {id: 'A-MoreOOP', title: 'Use More OOP'}
  ]},
    {id: 'add_increments', suffix: ' as PRs', increments:  [
    {id: 'Level-8', title: 'Dates and Times', tag: 'optional'},
    {id: 'Level-9', title: 'Find'},
    {id: 'A-JUnit', title: 'Add JUnit Tests'}
  ]}
],
week7: [
  {id: 'set_up_website'},
  {id: 'submit_the_final_version', deadline: get_date(date_w7_start, 10)}
]
} %}
