## Hi there 👋

<!--
**studyprox/studyprox** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-
// learnhub-templates/CourseDashboard.jsx
import React from 'react';
import { AIStudyAssistant } from '../ai-templates/AIComponents';

const CourseDashboard = ({ courses, userProgress }) => {
  return (
    <div className="lms-dashboard">
      <h2>My Learning Dashboard</h2>
      
      <div className="ai-assistant-section">
        <AIStudyAssistant context="course-dashboard" />
      </div>
      
      <div className="course-grid">
        {courses.map(course => (
          <CourseCard 
            key={course.id}
            course={course}
            progress={userProgress[course.id]}
          />
        ))}
      </div>
    </div>
  );
};
