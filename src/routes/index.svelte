<script>
  import {
    Header04,
    Text00,
    Text01,
    Text04,
    Features01,
    Pricing01,
    Testimonials01,
    EmailForm03,
    FAQ02,
    Contact02,
    Banner,
    Nav01
  } from "../unicorn";
  // export let name;
  const features = [
    {
      title: "Charlemos",
      description:
        "Las comunidades hablan. Ya sea Slack, nuestra página de Facebook, Instagram, o incluso email, estamos ahí para escuchar tus dudas y leer tus memes.",
      img: "img/icons/abstract_icons/abstract-icon-6.svg"
    },
    {
      title: "Experiencias Colaborativas",
      description:
        "Creemos que es mejor aprender, construir y crecer en equipo. Catalizamos estos procesos con eventos colaborativos.",
      img: "img/icons/abstract_icons/abstract-icon-5.svg"
    },
    {
      title: "Eventos del tamaño de tu pasión",
      description:
        "Hacemos eventos de 20+ horas porque estamos locos y tú también. Creamos cosas y hackeamos el mundo.",
      img: "img/icons/abstract_icons/abstract-icon-8.svg"
    },
    {
      title: "Conexiones",
      description:
        "Nuestra red de patrocinadores, colaboradores y miembros es nustro recurso más importante. Sácale provecho, te ayudamos.",
      img: "img/icons/abstract_icons/abstract-icon-9.svg"
    },
    {
      title: "Cursos",
      description:
        "Ya sea para conocer sobre Machine Learning, o los básicos de programación, a nadie nos viene mal algo de aprendizaje.",
      img: "img/icons/abstract_icons/abstract-icon-11.svg"
    },
    {
      title: "Beneficios para Hackers",
      description:
        "Perks, red de expertos, incubadora de empresas, área de coworking, conexiones con Startups,y muchas más cosas que a ningún Hacker le vienen mal. ",
      img: "img/icons/abstract_icons/abstract-icon-12.svg"
    }
  ];
  const cards = [
    {
      main: "Developer",
      sub:
        "Si eres un would-be Hacker y quieres aprender todas las de la programación.",
      img: "img/emoji/scooter.png",
      prices: [99, 79],
      items: ["Cursos a $100", "Bootcamps a $250", "Hackathones a $350"],
      button: { title: "Start Now", link: "/" }
    },
    {
      main: "Hacker",
      sub:
        "Si quieres ir a todos los eventos y tienes alguans ideas para cambiar el mundo.",
      img: "img/emoji/motorcycle.png",
      prices: [399, 299],
      items: [
        "Cursos a $50",
        "Bootcamps a $150",
        "Hackathones a $300",
        "Accesso a red de expertos Nova Orión",
        "Descuento Coworking Tec 50%"
      ],
      button: { title: "Start Now", link: "/" }
    },
    {
      main: "Gangster",
      sub: "Si lo tuyo es quererlo todo y cambiar el mundo en el proceso.",
      img: "img/emoji/jet.png",
      prices: [599, 499],
      items: [
        "Cursos a $0",
        "Bootcamps a $50",
        "Hackathones a $100",
        "Descuento en Coworking Tec de 100%",
        "Programa Work at a Startup",
        "Beca en Incubación de Nova Orión"
      ],
      button: { title: "Start Now", link: "/" }
    }
  ];
  const faqs = [
    {
      q: "¿Qué es Hacker Mafia Club?",
      a:
        "<p>Hacker Mafia Club es una comunidad que nació en el Parque Tecnológico Orión con e fin de crear una comunidad de personas técnicas que disfruten aprender, investigar y trabajar en áreas de software, específicamente de Machine Learning.</p>"
    },
    {
      q: "¿Qué tecnologías usan?",
      a:
        "<p>Somos una comunidad de software, y por lo mismo usamos todas las tecnologías que puedan llegar a compilar en algún ambiente de desarrollo, no obstante, por nuestro enfoque en Machine Learning y nuestro interés por atraer gente de otras áreas, usamos Python por su gran repertorio de librerías y su facilidad de aprendizaje.</p>"
    },
    {
      q: "¿Qué necesito para formar parte?",
      a:
        ' <p>Estar interesado. Muchos de nuestro eventos no tienen costo, pero como queremos crecer esta comunidad y los hackers no comemos aire, algunos otros sí. </p> <p>Buscamos dismuniur el costo de atendencia a través de nuestro programa de <a href="javascript:void(0)">suscripciones</a>, y de ser necesario podemos evaluar casos espcíficos a través de <a href="mailto:hackermafia@orionstartups.com?subject=Proceso%20de%20beca">becas</a>.</p>'
    },
    {
      q: "¿Dónde están ubicados?",
      a:
        '<p>Nuestros "cuarteles generales" están ubicados en las oficinas de Orion Startups, piso 6to del PIT 3 en el Parque Orión.</p> <p>Sin embargo, muchos de nuestros eventos toman lugar fuera del Parque Orión y dentro de otras universidades aliadas.</p>'
    }
  ];
  const icons = [
    {
      img: "img/icons/social/black/slack.svg",
      link:
        "https://join.slack.com/t/hacker-mafia/shared_invite/enQtNjgzMzQwMzA3MDcyLTQ3ZmM0ZTVhNzEwYjFlM2QyYzA5NTc3M2M0NjIwY2Y0Y2ZkZmFlNmM3ODZmMDE4YWQ1NmM1YWRjZmZmOTY0MGY",
      platform: "Slack"
    },
    {
      img: "img/icons/social/black/facebook.svg",
      link: "https://www.facebook.com/Hacker-Mafia-386592791984319/",
      platform: "Facebook"
    },
    {
      img: "img/icons/social/black/twitter.svg",
      link: "https://twitter.com/hackermafiaclub",
      platform: "Twitter"
    },
    {
      img: "img/icons/social/black/instagram.svg",
      link: "javascript:alert('coming soon')",
      platform: "Instagram"
    },
    {
      img: "img/icons/social/black/medium1.svg",
      link: "https://medium.com/hacker-mafia-club",
      platform: "Medium"
    }
  ];
</script>

<style>

</style>

<!-- <svelte:head>
  <title>Home</title>
</svelte:head> -->

<div style="margin-top: -120px">
  <Header04
    main="Una comunidad de Hackers para Hackers"
    sub="Hacker Mafia es una comunidad para todos aquellos Hackers que creemos
    en cambiar el mundo software y la inteligencia artificial. <br />Made with
    ❤️ in Chihuahua"
    img="img/photos/cool-laptop.jpeg"
    buttons={[{ title: 'Sign up', link: '/' }, { title: 'Learn more' }]} />
  <Text04
    text="Porque Chihuahua está lista para una comunidad técnica de Inteligencia
    Artificial y Software." />
  <Features01
    main="Holístico y para todos"
    sub="Crecemos contigo y hay eventos para todo nivel de entusiasta. Desde
    algunos meses hasta algunos doctorados."
    {features} />
  <Text01
    cards={['"Muy buena organización y participación por parte de los organizadores como de los participantes, imposible salir sin aprender nada."', '"Muy padre, así como la organización por parte del staff. La convivencia con los demás participantes fue muy agradable y me gustó mucho."']} />
  <Pricing01
    main="Escoge tu plan"
    sub="Subscripciones para Hackers de todo tamaño, ambición e intereses."
    tabs={['Mensual', 'Anual']}
    badgeText="+1 mes gratis"
    {cards} />
  <Text00
    main="¿No estás seguro?"
    sub="Asiste a nuestros eventos para que no te cuenten. A costo de público."
    items={['Cursos: $200', 'Bootcamps: $300', 'Hackathones: $400']} />
  <Testimonials01
    main="Nuestros Patrocinadores"
    sub="Sin ellos Hacker Mafia sería solo una idea en la mente de todos
    nosotros." />
  <EmailForm03
    main="¿Quieres saber más?"
    sub="Inscríbete a nuestra mailing list.<br />No se requiere nada."
    placeholder="Danos tu email"
    buttonTitle="Subscríbete" />
  <FAQ02
    main="Tú Preguntas, Nosotros Contestamos"
    sub="Preguntar es de sabios, pero nadie se a ha muerto por leer un FAQ."
    {faqs}
    help="¿No ves tu pregunta?"
    button={{ title: 'Mándanos un mail', link: 'mailto:hackermafia@orionstartups.com?subject=Pregunta%20Hacker' }} />
  <Contact02
    main="Síguenos"
    contacts={[{ title: 'Contacto', email: 'hackermafia@orionstartups.com' }]}
    {icons} />
  <Banner />
</div>
