<template>
  <div class="flex flex-col w-screen h-full">
    <!-- Your name, profile picture and contact -->
    <HeadWrapper
      name="muhammada fahmi"
      title="Your Job Title"
      userImgURL="../img/github.png"
      phone="011-37553548"
      email="muhammadfahmi@gmail.com"
    />
    <!-- About Me -->
    <AboutWrapper
      aboutMe="Heloo i am Muhammad Fahmi .Age 25 this year"
      linkedInURL="Your LinkedIn URL Address"
      languages="malay"
      nationality="Malaysia"
      interest="Sleeping"
    />
    <!-- Working Experience -->
    <CareerWrapper>
      <template v-slot:career>
        <Career companyName="OUM" title="Student" startDate="Start Date" endDate="End Date">
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>

        <Career companyName="Las Vacas" title="Kitchen Helper" startDate="2016" endDate="2018">
          <!-- List of what you had did in the company -->
          <template v-slot:experience>
            <ul class="text-gray-600 list-inside list-disc mt-2 px-4">
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
              <li>Lorem, ipsum dolor sit amet consectetur adipisicing elit. A, nihil. Aut sapiente ipsa fugiat quasi nisi officiis cumque, amet enim corporis. Pariatur distinctio maxime sint, ducimus quos quia nostrum atque.</li>
            </ul>
          </template>
        </Career>
      </template>
    </CareerWrapper>
    <!-- Achievement -->
    <AchievementWrapper project="1" client=" 1  " award="1"/>
    <!-- Portfolio -->
    <PortfolioWrapper>
      <template v-slot:portfolio>
        <div class="grid grid-cols-1 md:grid-cols-3">
          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />

          <ProjectCard
            imgUrl="../img/github.png"
            name="Project Name"
            project="Project Type"
            projectURL="https://github.com"
          />
        </div>
      </template>
    </PortfolioWrapper>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "Fahmi..."
    };
  }
};
</script>