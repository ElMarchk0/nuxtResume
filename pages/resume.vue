<template>
  <NuxtLayout name="default">
    <h1 class="text-center text-4xl my-4">Resume</h1>
    <a
      class="flex justify-center text-xl hover:text-blue-400"
      download="Resume_Peter_Charlesworth.pdf"
      href="/Resume_Peter_Charlesworth.pdf"
      target="_blank"
      >Download a PDF of My Resume</a
    >

    <div
      class="flex flex-wrap lg:justify-center flex-cols-3 m-4 md:justify-start px-16"
    >
      <History title="Work" :data="history.workHistory" />
      <History title="Education" :data="history.educationHistory" />
      <Skills :data="history.skills" />
    </div>
  </NuxtLayout>
</template>

<style>
.category-title {
  @apply text-2xl font-bold;
}
</style>

<script>
export default {
  data() {
    return {
      history: {
        workHistory: [
          {
            title: "Product Data Administrator",
            company: "Andrew Sheret LTD",
            location: "Victoria, BC",
            date: "September 2023 - Current",
            description: [
              "Developed Python scripts to clean, analyze, and process product data provided by vendors and suppliers",
            ],
          },
          {
            title: "API Developer",
            company: "Indigenous Perspectives Society",
            location: "Victoria, BC",
            date: "May 2023 - August 2023",
            description: [
              "Worked with IPS members develop a data schema to track project data",
              "Served as lead developer for the backend API that was built with Django and MySQL",
              "Implemented hosting solutions for the API and the frontend web application",
            ],
          },
          {
            title: "Software Development Co-op",
            company: "Cognito Health",
            location: "Victoria, BC",
            date: "May 2022 - August 2022",
            description: [
              "Built and refactored UI components for production applications using React Typescript and ChakraUI",
              "Built and refactored testing suites for production React applications using Jest and the React testing library",
              "Built and refactored and maintained REST APIs using TypeScript, NestJs, TypeOrm and MySql",
              "Implemented google analytics for a production full-stack application",
              "Configured third party applications such as Auth0, Calendly, Google Analytics and Stripe for a full-stack production application",
              "Utilized git and GitHub for version control and project management within a team",
              "Performed code reviews and pull requests for team members",
            ],
          },
          {
            title: "Carpentry Apprentice",
            company: "Campbell Construction",
            location: "Victoria, BC",
            date: "February 2019 - August 2021",
            description: [
              "Built concrete forms according to engineered plans and federal building standards",
              "Laid out grid-lines and benchmarks according to engineered plans",
            ],
          },
          {
            title: "Carpentry Apprentice",
            company: "KD Johnson",
            location: "Victoria, BC",
            date: "June 2017 – August 2018",
            description: [
              "Collaborated with a large team and a large number of workers from other companies and different trades",
              "Built lumber frames and concrete forms according to engineered plans and federal building standards",
            ],
          },
          {
            title: "Laborer",
            company: "Walcan Seafoods",
            location: "Quadra Island, BC",
            date: "June 2012 – August 2016",
            description: [
              "Worked with a large crew of up to 50 people",
              "Supervised Crew of up to 15 people",
            ],
          },
        ],

        educationHistory: [
          {
            title: "Information and Computer Systems Diploma",
            school: "Camosun College",
            location: "Victoria, BC",
            date: "September 2020 - May 2022",
            description: [
              "Learned object orientated programming, abstract data structures and algorithm concepts with Java",
              "Built and maintained virtual machines and servers using Linux and Windows operating systems",
              "Wrote bash scripts and pythons scripts to maintain and automate system process",
              "Built a variety of frontend web pages and applications using CSS, HTML, JavaScript",
              "Learned applied computer science mathematics",
              "Learned applied database concepts and theory, built and maintained relational databases",
            ],
          },
          {
            title: "Carpentry Level One",
            school: "Camosun College",
            location: "Victoria, BC",
            date: "January 2019 - February 2019",
            description: [
              "Learned applied construction and building techniques",
              "Learned how to interpret provincial and federal building codes",
            ],
          },
          {
            title: "Electrical Trades Foundation",
            school: "Camosun College",
            location: "Victoria, BC",
            date: "November 2016 – May 2017",
            description: [
              "Assembled electrical circuits and motors",
              "Learned how to interpret provincial and federal building codes",
            ],
          },
        ],
        skills: [
          {
            title: "Frontend Web Technologies",
            description:
              "Bootstrap, Chakra UI, CSS, HTML, React, Tailwindcss, Vue.js",
          },
          {
            title: "Backend Web Technologies",
            description: "Django, Express, NestJS, Node.js",
          },
          {
            title: "Programming Lanuages",
            description: "C++, C#, Java, Javascript, Python, Swift, Typescript",
          },
          {
            title: "Networking & Infrastructure",
            description:
              "AWS, Docker, Git, Linux, Virtual Machines, Windows Server",
          },
          {
            title: "Databases",
            description: "MongoDB, MySQL, Oracle",
          },
        ],
      },
    };
  },
};
</script>
