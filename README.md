import React from 'react';
import Typing from 'react-typing-effect';
import { FaTwitter, FaLinkedin, FaInstagram, FaGithub } from 'react-icons/fa';
import { motion } from 'framer-motion';

export default function Home() {
  return (
    <div style={{ textAlign: 'center', padding: '2rem', fontFamily: 'sans-serif' }}>
      {/* Header */}
      <motion.h1 initial={{ opacity: 0 }} animate={{ opacity: 1 }} transition={{ duration: 1 }}>
        Hi there 👋, I'm Akash Maurya
      </motion.h1>
      <motion.h3 initial={{ opacity: 0 }} animate={{ opacity: 1 }} transition={{ delay: 0.5 }}>
        A passionate Frontend Developer from India
      </motion.h3>

      {/* Typing Animation */}
      <Typing
        text={[
          "Frontend Developer",
          "React Learner",
          "MySQL Explorer",
          "Always Learning New Things",
          "C Programmer"
        ]}
        speed={100}
        eraseSpeed={50}
        eraseDelay={1500}
        typingDelay={500}
        cursor="_"
      />

      {/* Social Icons */}
      <div style={{ margin: '2rem' }}>
        <a href="https://twitter.com/akash__dp" target="_blank" rel="noreferrer"><FaTwitter size={40} style={{ margin: '0 10px' }}/></a>
        <a href="https://linkedin.com/in/akash-maurya" target="_blank" rel="noreferrer"><FaLinkedin size={40} style={{ margin: '0 10px' }}/></a>
        <a href="https://instagram.com/akash__dp" target="_blank" rel="noreferrer"><FaInstagram size={40} style={{ margin: '0 10px' }}/></a>
        <a href="https://github.com/dp7772" target="_blank" rel="noreferrer"><FaGithub size={40} style={{ margin: '0 10px' }}/></a>
      </div>

      {/* About Me */}
      <motion.div
        initial={{ x: -200, opacity: 0 }}
        animate={{ x: 0, opacity: 1 }}
        transition={{ duration: 1 }}
        style={{ textAlign: 'left', maxWidth: '600px', margin: 'auto' }}
      >
        <h3>💡 About Me</h3>
        <ul>
          <li>🔭 I’m currently working on <b>React Animation Website</b></li>
          <li>🌱 I’m currently learning <b>MySQL, React, Tailwind</b></li>
          <li>👨‍💻 All of my projects are available at <a href="https://akashmaurya.netlify.app">My Portfolio</a></li>
          <li>💬 Ask me about <b>HTML, CSS, CSS3, JavaScript, Bootstrap, C</b></li>
          <li>⚡ Fun fact: I think imagination is the best tool for a coder</li>
        </ul>
      </motion.div>

      {/* Animated Tech Stack */}
      <motion.div
        initial={{ y: 100, opacity: 0 }}
        animate={{ y: 0, opacity: 1 }}
        transition={{ duration: 1, delay: 1 }}
      >
        <h3>🛠️ Languages & Tools</h3>
        <img src="https://skillicons.dev/icons?i=html,css,js,bootstrap,mysql,c,git,github,vscode" alt="Tech Stack"/>
      </motion.div>

      {/* Projects */}
      <motion.div
        initial={{ scale: 0.8, opacity: 0 }}
        animate={{ scale: 1, opacity: 1 }}
        transition={{ duration: 1, delay: 1.5 }}
      >
        <h3>🚀 Projects</h3>
        <a href="https://akashmaurya.netlify.app/react-animation-website" target="_blank" rel="noreferrer">
          <button style={{ margin: '5px', padding: '10px 20px', cursor: 'pointer' }}>React Animation Website</button>
        </a>
        <a href="https://akashmaurya.netlify.app/weather-app" target="_blank" rel="noreferrer">
          <button style={{ margin: '5px', padding: '10px 20px', cursor: 'pointer' }}>Weather App</button>
        </a>
        <a href="https://akashmaurya.netlify.app/portfolio" target="_blank" rel="noreferrer">
          <button style={{ margin: '5px', padding: '10px 20px', cursor: 'pointer' }}>Portfolio</button>
        </a>
      </motion.div>
    </div>
  );
}
