import React from 'react';
import { Card, CardContent } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { FaLinkedin, FaGithub, FaEnvelope } from 'react-icons/fa';
import { motion } from 'framer-motion';

const Portfolio = () => {
    return (
        <div className="bg-gray-900 text-white min-h-screen">
            <header className="p-8 bg-gray-800 text-center">
                <h1 className="text-5xl font-bold mb-2">Akhil Vallala</h1>
                <p className="text-xl text-gray-400">Data Scientist | Machine Learning Engineer | AI Enthusiast</p>
                <div className="flex justify-center gap-4 mt-4">
                    <a href="https://www.linkedin.com/in/akhil-fau" target="_blank" className="text-blue-500 text-3xl"><FaLinkedin /></a>
                    <a href="https://github.com/akhilfau" target="_blank" className="text-gray-300 text-3xl"><FaGithub /></a>
                    <a href="mailto:avallala2023@fau.edu" className="text-red-400 text-3xl"><FaEnvelope /></a>
                </div>
            </header>

            <section className="p-8">
                <h2 className="text-4xl font-bold mb-4">About Me</h2>
                <p className="text-lg text-gray-300 mb-6">
                    I am a passionate Data Scientist pursuing my Master’s in Data Science at Florida Atlantic University. My work spans data analytics, machine learning, and AI, with a focus on educational technology and natural language processing. With experience in fine-tuning language models and developing AI-driven solutions, I aim to create impactful, data-driven systems for real-world applications.
                </p>
                <Button className="bg-blue-500 hover:bg-blue-600">Download Resume</Button>
            </section>

            <section className="p-8 bg-gray-800">
                <h2 className="text-4xl font-bold mb-4">Skills</h2>
                <ul className="text-lg text-gray-300 mb-6">
                    <li>Programming: Python, PySpark, SQL, Git</li>
                    <li>Data Analytics: Pandas, NumPy, Power BI, Matplotlib</li>
                    <li>Machine Learning: LLM Training, Deep Learning, Prompt Engineering</li>
                    <li>Data Visualization: Power BI, Tableau</li>
                    <li>Cloud Technologies: Azure Data Factory, Azure DevOps</li>
                </ul>
            </section>

            <section className="p-8">
                <h2 className="text-4xl font-bold mb-4">Projects</h2>
                <Card className="mb-4">
                    <CardContent>
                        <h3 className="text-2xl font-semibold">PhysmolLM</h3>
                        <p className="text-gray-300">
                            Developed a compact language model for enhancing physics education, fine-tuned with custom datasets for improved question-answering performance.
                        </p>
                    </CardContent>
                </Card>
                <Card className="mb-4">
                    <CardContent>
                        <h3 className="text-2xl font-semibold">Academic Responsible Assistant (ARA)</h3>
                        <p className="text-gray-300">
                            Built an AI-driven solution to proactively prevent academic cheating using Retrieval-Augmented Generation (RAG) with Streamlit UI.
                        </p>
                    </CardContent>
                </Card>
            </section>

            <section className="p-8 bg-gray-800">
                <h2 className="text-4xl font-bold mb-4">Contact</h2>
                <p className="text-lg text-gray-300 mb-6">Let's connect and explore AI opportunities together!</p>
                <Button className="bg-blue-500 hover:bg-blue-600">Get in Touch</Button>
            </section>

            <footer className="p-4 bg-gray-900 text-center text-gray-500">
                © 2025 Akhil Vallala. All Rights Reserved.
            </footer>
        </div>
    );
};

export default Portfolio;
