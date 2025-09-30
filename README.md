import React from "react";

// Portfolio - Single-file React component
// Tailwind CSS utility classes assumed to be available in your project
// Default export so this can be used as a page (e.g. in GitHub Pages with a simple React build)

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gray-50 text-gray-900 font-sans">
      <header className="container mx-auto px-6 py-8 flex items-center justify-between">
        <div>
          <h1 className="text-2xl md:text-3xl font-bold">Mohamed TA</h1>
          <p className="text-sm md:text-base text-gray-600">Monitoring, Evaluation & Learning (MEL) Analyst • Data Analyst</p>
        </div>
        <nav className="space-x-4 text-sm">
          <a href="#projects" className="hover:underline">Projects</a>
          <a href="#skills" className="hover:underline">Skills</a>
          <a href="#about" className="hover:underline">About</a>
          <a href="#contact" className="hover:underline">Contact</a>
        </nav>
      </header>

      <main className="container mx-auto px-6">
        {/* Hero */}
        <section className="bg-white rounded-2xl shadow p-6 md:p-10 mb-8 flex flex-col md:flex-row items-center gap-6">
          <div className="flex-1">
            <h2 className="text-2xl md:text-4xl font-extrabold mb-3">Je transforme les données en apprentissages pour maximiser l’impact</h2>
            <p className="text-gray-600 mb-4">Je conçois des systèmes de suivi-évaluation, développe des tableaux de bord interactifs et analyse les données pour aider les équipes à prendre des décisions fondées sur des preuves.</p>
            <div className="flex gap-3">
              <a href="#projects" className="inline-block px-4 py-2 bg-indigo-600 text-white rounded-md">Voir mes projets</a>
              <a href="/cv.pdf" className="inline-block px-4 py-2 border border-indigo-600 text-indigo-600 rounded-md">Télécharger CV</a>
            </div>
          </div>
          <div className="w-48 h-48 md:w-56 md:h-56 bg-indigo-50 rounded-xl flex items-center justify-center">
            <div className="text-center text-sm text-gray-500">Photo / avatar<br/>(remplace par la tienne)</div>
          </div>
        </section>

        {/* About */}
        <section id="about" className="mb-8">
          <div className="bg-white rounded-2xl shadow p-6">
            <h3 className="text-xl font-semibold mb-3">À propos de moi</h3>
            <p className="text-gray-700 leading-relaxed">Je suis Monitoring, Evaluation & Learning Analyst passionné par la donnée comme levier de décision et d’impact. J’aide les organisations à mesurer leurs résultats, analyser leurs données et capitaliser les apprentissages. J’ai une expérience pratique sur Excel avancé, Power BI, Python et SQL, ainsi que sur les méthodologies MEL (logframe, ToC, indicateurs, évaluations mixtes).</p>
          </div>
        </section>

        {/* Skills */}
        <section id="skills" className="mb-8 grid md:grid-cols-3 gap-6">
          <div className="bg-white rounded-2xl shadow p-6">
            <h4 className="font-semibold mb-2">Monitoring & Evaluation</h4>
            <ul className="text-gray-600 list-disc ml-5">
              <li>Cadres de résultats (logframe, ToC)</li>
              <li>Conception d’indicateurs</li>
              <li>Collecte & qualité des données (Kobo, ODK)</li>
              <li>Évaluations qualitatives & quantitatives</li>
            </ul>
          </div>

          <div className="bg-white rounded-2xl shadow p-6">
            <h4 className="font-semibold mb-2">Data & Visualisation</h4>
            <ul className="text-gray-600 list-disc ml-5">
              <li>Excel avancé (Power Query, Pivot, DAX)</li>
              <li>Power BI • Tableau • Looker Studio</li>
              <li>SQL • Python (pandas)</li>
              <li>Nettoyage de données & automatisation</li>
            </ul>
          </div>

          <div className="bg-white rounded-2xl shadow p-6">
            <h4 className="font-semibold mb-2">Soft skills</h4>
            <ul className="text-gray-600 list-disc ml-5">
              <li>Communication aux parties prenantes</li>
              <li>Formation & transfert de compétences</li>
              <li>Gestion de projets</li>
              <li>Rigueur analytique</li>
            </ul>
          </div>
        </section>

        {/* Projects */}
        <section id="projects" className="mb-12">
          <h3 className="text-xl font-semibold mb-4">Projets & Études de cas</h3>
          <div className="grid md:grid-cols-3 gap-6">
            {/* Project 1 */}
            <article className="bg-white rounded-2xl shadow p-5">
              <h4 className="font-semibold mb-2">Tableau de bord Power BI</h4>
              <p className="text-gray-600 mb-3">Consolidation des données de 5 régions et construction d’un dashboard interactif pour le suivi d’indicateurs.</p>
              <ul className="text-sm text-gray-600 list-disc ml-5 mb-3">
                <li>Réduction du temps de reporting de 40%</li>
                <li>Outils : Excel, Power BI, SQL</li>
              </ul>
              <a className="text-indigo-600 text-sm hover:underline" href="#">Voir détail / capture</a>
            </article>

            {/* Project 2 */}
            <article className="bg-white rounded-2xl shadow p-5">
              <h4 className="font-semibold mb-2">Évaluation d’impact (formation pro)</h4>
              <p className="text-gray-600 mb-3">Enquête Kobo et analyse sous Python pour mesurer l’effet d’une formation sur l’insertion.</p>
              <ul className="text-sm text-gray-600 list-disc ml-5 mb-3">
                <li>Augmentation de 25% du taux d’insertion observée</li>
                <li>Outils : Kobo, Python</li>
              </ul>
              <a className="text-indigo-600 text-sm hover:underline" href="#">Voir détail / capture</a>
            </article>

            {/* Project 3 */}
            <article className="bg-white rounded-2xl shadow p-5">
              <h4 className="font-semibold mb-2">Automatisation du reporting</h4>
              <p className="text-gray-600 mb-3">Système Excel + Power Query pour automatiser les rapports mensuels d’une ONG locale.</p>
              <ul className="text-sm text-gray-600 list-disc ml-5 mb-3">
                <li>Gain : 10 heures / mois</li>
                <li>Outils : Excel, Power Query</li>
              </ul>
              <a className="text-indigo-600 text-sm hover:underline" href="#">Voir détail / capture</a>
            </article>
          </div>
        </section>

        {/* Publications */}
        <section className="mb-12">
          <div className="bg-white rounded-2xl shadow p-6">
            <h3 className="text-xl font-semibold mb-3">Publications & Contributions</h3>
            <ul className="list-disc ml-5 text-gray-600">
              <li>Rapport de suivi annuel — Organisation X (2024)</li>
              <li>Présentation : « Utiliser la donnée pour améliorer l’impact » (2025)</li>
              <li>Article interne : 5 bonnes pratiques pour un reporting MEL efficace</li>
            </ul>
          </div>
        </section>

        {/* Contact */}
        <section id="contact" className="mb-20">
          <div className="bg-white rounded-2xl shadow p-6 md:flex md:items-center md:justify-between">
            <div>
              <h3 className="text-xl font-semibold">Contact</h3>
              <p className="text-gray-600">Intéressé par une collaboration ou une mission ? Écris-moi.</p>
              <ul className="mt-3 text-gray-600">
                <li>Email: <a href="mailto:youremail@example.com" className="text-indigo-600 hover:underline">youremail@example.com</a></li>
                <li>LinkedIn: <a href="https://www.linkedin.com" className="text-indigo-600 hover:underline">linkedin.com/in/tonprofil</a></li>
                <li>GitHub: <a href="https://github.com" className="text-indigo-600 hover:underline">github.com/tonprofil</a></li>
              </ul>
            </div>
            <div className="mt-6 md:mt-0">
              <a href="/cv.pdf" className="inline-block px-4 py-2 bg-indigo-600 text-white rounded-md">Télécharger CV</a>
            </div>
          </div>
        </section>

      </main>

      <footer className="py-6">
        <div className="container mx-auto px-6 text-center text-sm text-gray-500">© {new Date().getFullYear()} Mohamed TA — Monitoring, Evaluation & Learning • Data Analyst</div>
      </footer>
    </div>
  );
}
transformer les données en histoires qui génèrent de l’impact. »*
