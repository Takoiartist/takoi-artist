/* =====================================================
   TAKOI STUDIO — script.js
   Bilingual landing page logic: i18n, portfolio filters,
   dynamic pricing, interactive wizard brief, FAQ, modals.
===================================================== */
(function () {
  "use strict";

  var PLACEHOLDER_IMG =
    "data:image/svg+xml;charset=UTF-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='320'%3E%3Crect width='400' height='320' fill='%23F4F0FA'/%3E%3Ctext x='50%25' y='50%25' font-family='sans-serif' font-size='16' fill='%236E3FA8' text-anchor='middle' dominant-baseline='middle'%3EImagen no disponible%3C/text%3E%3C/svg%3E";

  function withFallback(img) {
    img.addEventListener(
      "error",
      function () {
        img.onerror = null;
        img.src = PLACEHOLDER_IMG;
      },
      { once: true }
    );
    return img;
  }

  /* =====================================================
     TRANSLATIONS — static UI strings (data-i18n keys)
  ===================================================== */
  var UI = {
    es: {
      "nav.services": "Servicios",
      "nav.catalog": "Brand Identity",
      "nav.portfolio": "Portafolio",
      "nav.pricing": "Paquetes",
      "nav.brief": "Brief",
      "nav.faq": "FAQ",
      "nav.contact": "Contacto",
      "nav.whatsapp": "WhatsApp",
      "nav.email": "Escribir un correo",
      "hero.kicker": "Estudio de branding independiente",
      "hero.title": "Branding que hace que tu marca sea reconocible.",
      "hero.text":
        "Creamos logos, identidades visuales y sistemas de marca pensados para comunicar tu esencia, conectar con tu audiencia y hacer crecer tu negocio.",
      "hero.btn1": "Ver servicios",
      "hero.btn2": "Hablar por WhatsApp",
      "services.title": "Servicios de diseño",
      "services.logo.title": "Logo Design",
      "services.logo.text": "Un símbolo memorable, construido desde cero para tu marca.",
      "services.brand.title": "Brand Identity",
      "services.brand.text": "Sistema visual completo: logo, paleta, tipografía y aplicaciones.",
      "services.complete.title": "Complete Branding",
      "services.complete.text": "Identidad completa lista para lanzar tu marca al mercado.",
      "services.social.title": "Social Media Design",
      "services.social.text": "Piezas gráficas coherentes para tus redes sociales.",
      "services.guidelines.title": "Brand Guidelines",
      "services.guidelines.text": "El manual que asegura que tu marca se use siempre bien.",
      "services.more": "Ver más →",
      "catalog.title": "Catálogo de Brand Identity",
      "catalog.text": "Sistemas de identidad de marca organizados por temática, con ejemplos reales de trabajo.",
      "logos.title": "Logos seleccionados",
      "logos.text":
        "Una selección de identidades y logos desarrollados para diferentes tipos de marcas y proyectos.",
      "logos.filter.all": "Todos",
      "logos.filter.logos": "Logos",
      "logos.filter.identity": "Brand Identity",
      "logos.filter.design": "Brand Design",
      "logos.viewall": "Ver portafolio completo",
      "brandid.title": "Proyectos de identidad de marca",
      "brandid.text":
        "Sistemas completos de marca desarrollados de principio a fin: investigación, logo, manual y aplicaciones.",
      "pricing.title": "Nuestros paquetes",
      "pricing.text":
        "Precios en USD para clientes de Florida y Estados Unidos. Equivalente aproximado en COP como referencia.",
      "pricing.group.logos": "Diseño de logo",
      "pricing.group.guidelines": "Manuales de marca",
      "pricing.group.identity": "Paquetes de identidad de marca",
      "pricing.group.social": "Social Media Design",
      "pricing.terms":
        "50% de anticipo para iniciar el proyecto. 50% restante al finalizar y antes de la entrega de los archivos editables, cuando estén incluidos en el paquete.",
      "pricing.note":
        "Cada servicio incluye el número de rondas de modificaciones especificado en su descripción. Modificaciones adicionales o cambios sustanciales podrán generar un costo adicional.",
      "brief.title": "Cuéntame sobre tu proyecto",
      "brief.text": "Responde algunas preguntas para que pueda entender tu marca antes de empezar.",
      "brief.back": "Atrás",
      "brief.next": "Siguiente",
      "brief.submit": "Enviar brief",
      "brief.success.title": "¡Gracias por compartir tu proyecto!",
      "brief.success.text":
        "Hemos recibido tu brief. Revisaremos la información y nos pondremos en contacto contigo para hablar sobre los próximos pasos.",
      "brief.success.whatsapp": "Hablar por WhatsApp",
      "brief.success.home": "Volver al inicio",
      "why.title": "¿Por qué trabajar conmigo?",
      "faq.title": "Preguntas frecuentes",
      "finalcta.title": "¿Listo para construir tu marca?",
      "finalcta.text":
        "Cuéntame sobre tu proyecto y encontremos el servicio adecuado para llevar tu identidad al siguiente nivel.",
      "finalcta.btn1": "Completar brief",
      "finalcta.btn2": "Hablar por WhatsApp",
      "footer.tag": "Diseño que impulsa tus ideas.",
      "modal.cta": "Solicitar este servicio",
      "modal.viewpdf": "Ver PDF"
    },
    en: {
      "nav.services": "Services",
      "nav.catalog": "Brand Identity",
      "nav.portfolio": "Portfolio",
      "nav.pricing": "Pricing",
      "nav.brief": "Brief",
      "nav.faq": "FAQ",
      "nav.contact": "Contact",
      "nav.whatsapp": "WhatsApp",
      "nav.email": "Send an email",
      "hero.kicker": "Independent branding studio",
      "hero.title": "Branding that makes your brand recognizable.",
      "hero.text":
        "We create logos, visual identities and brand systems designed to communicate your essence, connect with your audience and help your business grow.",
      "hero.btn1": "Explore services",
      "hero.btn2": "Chat on WhatsApp",
      "services.title": "Design services",
      "services.logo.title": "Logo Design",
      "services.logo.text": "A memorable mark, built from scratch for your brand.",
      "services.brand.title": "Brand Identity",
      "services.brand.text": "A complete visual system: logo, palette, typography and applications.",
      "services.complete.title": "Complete Branding",
      "services.complete.text": "A full identity, ready to bring your brand to market.",
      "services.social.title": "Social Media Design",
      "services.social.text": "Consistent graphic pieces for your social channels.",
      "services.guidelines.title": "Brand Guidelines",
      "services.guidelines.text": "The manual that keeps your brand used the right way.",
      "services.more": "See more →",
      "catalog.title": "Brand Identity Catalog",
      "catalog.text": "Brand identity systems organized by theme, with real work examples.",
      "logos.title": "Selected logo work",
      "logos.text": "A selection of logos and visual identities developed for different brands and projects.",
      "logos.filter.all": "All",
      "logos.filter.logos": "Logos",
      "logos.filter.identity": "Brand Identity",
      "logos.filter.design": "Brand Design",
      "logos.viewall": "View full portfolio",
      "brandid.title": "Brand identity projects",
      "brandid.text":
        "Complete brand systems built from start to finish: research, logo, manual and applications.",
      "pricing.title": "Branding packages",
      "pricing.text":
        "Prices in USD for clients in Florida and the United States. Approximate COP equivalent shown as reference.",
      "pricing.group.logos": "Logo design",
      "pricing.group.guidelines": "Brand manuals",
      "pricing.group.identity": "Brand identity packages",
      "pricing.group.social": "Social Media Design",
      "pricing.terms":
        "50% deposit to start the project. 50% remaining upon completion and before delivery of final editable files, when included in the package.",
      "pricing.note":
        "Each service includes the number of revision rounds specified in its description. Additional modifications or substantial changes may incur an extra cost.",
      "brief.title": "Tell me about your project",
      "brief.text": "Answer a few questions so I can understand your brand before we start.",
      "brief.back": "Back",
      "brief.next": "Next",
      "brief.submit": "Submit brief",
      "brief.success.title": "Thank you for sharing your project!",
      "brief.success.text":
        "We've received your brief. We'll review the information and get in touch with you to discuss the next steps.",
      "brief.success.whatsapp": "Chat on WhatsApp",
      "brief.success.home": "Back to home",
      "why.title": "Why work with Takoi?",
      "faq.title": "Frequently asked questions",
      "finalcta.title": "Ready to build your brand?",
      "finalcta.text": "Tell me about your project and let's find the right service to take your brand to the next level.",
      "finalcta.btn1": "Start your brief",
      "finalcta.btn2": "Chat on WhatsApp",
      "footer.tag": "Design that drives your ideas.",
      "modal.cta": "Request this service",
      "modal.viewpdf": "View PDF"
    }
  };

  var state = { lang: "es", filter: "all" };
  function t(key) {
    return (UI[state.lang] && UI[state.lang][key]) || key;
  }
  function L(obj) {
    return obj[state.lang] || obj.es;
  }

  /* =====================================================
     SERVICE MODAL DATA (Services section)
  ===================================================== */
  var SERVICE_DETAILS = {
    "logo-design": {
      title: { es: "Logo Design", en: "Logo Design" },
      text: {
        es: "Un logo construido desde la investigación de tu marca, no desde una plantilla. Elige entre tres niveles según cuántas propuestas y rondas de ajuste necesites.",
        en: "A logo built from real research on your brand, not a template. Choose between three tiers depending on how many concepts and revision rounds you need."
      },
      list: {
        es: ["Tipografía y símbolo a la medida", "Hasta 3 propuestas de logo", "Hasta 3 rondas de ajustes", "Archivos finales en PNG, JPG, PDF y SVG"],
        en: ["Custom typography and symbol", "Up to 3 logo concepts", "Up to 3 revision rounds", "Final files in PNG, JPG, PDF and SVG"]
      }
    },
    "brand-identity": {
      title: { es: "Brand Identity", en: "Brand Identity" },
      text: {
        es: "El sistema visual completo detrás de tu logo: paleta de colores, tipografía, iconografía básica y una guía de uso para mantener tu marca coherente.",
        en: "The complete visual system behind your logo: color palette, typography, basic iconography and a usage guide to keep your brand consistent."
      },
      list: {
        es: ["Concepto visual de marca", "Logo principal y secundario", "Paleta de colores y sistema tipográfico", "Guía de identidad visual", "Imagen de perfil para redes sociales"],
        en: ["Brand visual concept", "Primary and secondary logo", "Color palette and typography system", "Visual identity guide", "Profile image for social media"]
      }
    },
    "complete-branding": {
      title: { es: "Complete Branding", en: "Complete Branding" },
      text: {
        es: "Todo lo que necesitas para lanzar tu marca al mercado: identidad, manual profesional, papelería y piezas para redes sociales.",
        en: "Everything you need to bring your brand to market: identity, professional manual, stationery and social media pieces."
      },
      list: {
        es: ["Identidad de marca completa", "Manual profesional de marca", "Tarjeta de presentación y papelería básica", "5 plantillas para redes sociales", "Archivos editables y finales"],
        en: ["Complete brand identity", "Professional brand manual", "Business card and basic stationery", "5 social media templates", "Editable and final files"]
      }
    },
    "social-media": {
      title: { es: "Social Media Design", en: "Social Media Design" },
      text: {
        es: "Piezas gráficas puntuales o en lote para mantener tus redes sociales visualmente consistentes con tu marca.",
        en: "One-off or batched graphic pieces to keep your social channels visually consistent with your brand."
      },
      list: {
        es: ["Portada para Facebook", "Piezas individuales o en paquetes de 5 o 10", "Diseño adaptado a tu identidad existente", "Archivos finales listos para publicar"],
        en: ["Facebook cover", "Individual pieces or packs of 5 or 10", "Design adapted to your existing identity", "Final files ready to publish"]
      }
    },
    "brand-guidelines": {
      title: { es: "Brand Guidelines", en: "Brand Guidelines" },
      text: {
        es: "El manual que documenta cómo se usa tu marca: variantes de logo, colores exactos, tipografía y aplicaciones correctas e incorrectas.",
        en: "The manual documenting how your brand is used: logo variants, exact colors, typography, and correct and incorrect applications."
      },
      list: {
        es: ["Variantes de logo y logometría", "Colorimetría HEX, RGB y CMYK", "Tipografía y sistema gráfico", "Mockups de aplicación", "Usos correctos e incorrectos"],
        en: ["Logo variants and construction grid", "HEX, RGB and CMYK color codes", "Typography and graphic system", "Application mockups", "Correct and incorrect usage"]
      }
    }
  };

  /* =====================================================
     LOGO PORTFOLIO — real assets from takoiartist.github.io
  ===================================================== */
  var LOGOS = [
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/b28d5d955a7396165c6122c90ad877f404fa3cea/toro%20autos.webp",
      name: { es: "Toro Autos", en: "Toro Autos" },
      client: { es: "Alquiler de autos", en: "Car rental" },
      cat: "logos"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/83ff959fa81b7478e3b32b97f84976ded449f1ce/Sabor%20%26%20Vari%20Logo.png",
      name: { es: "Sabor & Vari", en: "Sabor & Vari" },
      client: { es: "Milkshakes", en: "Milkshakes" },
      cat: "logos"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/182cab60f1771b58f633d91652f2b0569750b6ff/Fivver%20Logos-06.png",
      name: { es: "Dachi Dana", en: "Dachi Dana" },
      client: { es: "Diseño de logo", en: "Logo design" },
      cat: "logos"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/182cab60f1771b58f633d91652f2b0569750b6ff/Fivver%20Logos-07.png",
      name: { es: "Renter Autos", en: "Renter Autos" },
      client: { es: "Alquiler de autos", en: "Car rental" },
      cat: "logos"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/83ff959fa81b7478e3b32b97f84976ded449f1ce/%5BJotako%5D%20Negos%20Logo%20Minimalista-07.png",
      name: { es: "Focus Box", en: "Focus Box" },
      client: { es: "Diseño de logo", en: "Logo design" },
      cat: "logos"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/83ff959fa81b7478e3b32b97f84976ded449f1ce/%5BJotako%5D%20Negos%20Logo%20Lettering-02.png",
      name: { es: "Rocca", en: "Rocca" },
      client: { es: "Gimnasio", en: "Gym" },
      cat: "logos"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/main/_PUNTOPET%20LOGO%2002.png",
      name: { es: "Punto Pet", en: "Punto Pet" },
      client: { es: "Logo de marca", en: "Brand logo" },
      cat: "logos"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/05498a0554493232152c3c31cb51157139bf022c/La%20Calma%20y%20Katanuchi_Mesa%20de%20trabajo%201.webp",
      name: { es: "La Calma y Katanuchi", en: "La Calma y Katanuchi" },
      client: { es: "Canal de YouTube", en: "YouTube channel" },
      cat: "logos"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/83ff959fa81b7478e3b32b97f84976ded449f1ce/%5BJotako%5D%20Negos%20Logo%20Ilustrado-12.png",
      name: { es: "Moto - Moto", en: "Moto - Moto" },
      client: { es: "Taller de motos", en: "Motorcycle repair shop" },
      cat: "brand-design"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/05498a0554493232152c3c31cb51157139bf022c/Viernes%20de%20Delicias_v3.0-06-convertido-de-jpg.webp",
      name: { es: "Delicias Santeñas", en: "Delicias Santeñas" },
      client: { es: "Branding de restaurante", en: "Restaurant branding" },
      cat: "brand-design"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/66fbbf42704583b718890dbc45c41b65eed6a56b/%5BJotako%5D%20Behance%20CCR-10-convertido-de-png.webp",
      name: { es: "CCR Brand Manual", en: "CCR Brand Manual" },
      client: { es: "Manual e identidad de marca", en: "Brand manual & identity" },
      cat: "brand-identity"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/7c500b3e2e3b110b00afb8ef2bfbb9d18d88fef3/%5BJotako%5D%20Behance%20Jotako%20Brand%202023_Mesa%20de%20trabajo%201.png",
      name: { es: "Jotako Brand Identity 2023", en: "Jotako Brand Identity 2023" },
      client: { es: "Identidad de marca propia", en: "In-house brand identity" },
      cat: "brand-identity"
    }
  ];

  var FILTER_LABELS = {
    logos: { es: "Logos", en: "Logos" },
    "brand-identity": { es: "Brand Identity", en: "Brand Identity" },
    "brand-design": { es: "Brand Design", en: "Brand Design" }
  };

  /* =====================================================
     BRAND IDENTITY EDITORIAL — the 3 real named projects
  ===================================================== */
  var BRAND_EDITORIAL = [
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/5ccb3576b72d7d9c295ea64ab4a34e87fc792454/manual%20de%20marca.webp",
      name: { es: "Brand Manual", en: "Brand Manual" },
      cat: { es: "Manual de marca", en: "Brand manual" },
      desc: {
        es: "Manual de marca desarrollado para documentar el uso correcto del logo, la paleta y la tipografía de un proyecto de branding.",
        en: "Brand manual developed to document the correct use of the logo, palette and typography for a branding project."
      },
      pdf: "https://drive.google.com/file/d/17CFDoviwSaygjhMp0ltyw1CwrUP4oEnt/view?usp=sharing"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/main/_PUNTOPET%20LOGO%2002.png",
      name: { es: "Punto Pet — Brandbook", en: "Punto Pet — Brandbook" },
      cat: { es: "Brandbook", en: "Brandbook" },
      desc: {
        es: "Brandbook con los logos editables y guías de aplicación desarrolladas para Punto Pet.",
        en: "Brandbook with editable logos and application guidelines developed for Punto Pet."
      },
      pdf:
        "https://docs.google.com/viewer?url=https%3A%2F%2Fraw.githubusercontent.com%2FTakoiartist%2Ftakoi-artist%2Fa81043f0e833ef8e213626830310b6116fd72b17%2FPUNTO%2520PET%2520EDITABLE%2520LOGOS.pdf&embedded=true"
    },
    {
      img: "https://raw.githubusercontent.com/Takoiartist/takoi-artist/main/manual%20de%20marca.webp",
      name: { es: "Dali Brand Identity 2023 — Manual", en: "Dali Brand Identity 2023 — Manual" },
      cat: { es: "Manual de marca", en: "Brand manual" },
      desc: {
        es: "Manual de identidad de marca desarrollado para el proyecto Dali, con sistema gráfico y guías de aplicación.",
        en: "Brand identity manual developed for the Dali project, including graphic system and application guidelines."
      },
      pdf:
        "https://docs.google.com/viewer?url=https%3A%2F%2Fraw.githubusercontent.com%2FTakoiartist%2Ftakoi-artist%2Ff62f983ea1b8aea4c5377824cc3172d34a43121f%2FMDM%2520DALI%252012.06.2020.pdf&embedded=true"
    }
  ];

  /* =====================================================
     PRICING DATA
  ===================================================== */
  var PRICING_LOGOS = [
    {
      name: { es: "Logo Básico", en: "Basic Logo" },
      num: "01",
      usd: "$110", cop: "≈ $350.000 COP",
      list: {
        es: ["Tipografía", "Símbolo", "1 propuesta de logo", "1 ronda de ajustes", "Archivos finales", "PNG, JPG, PDF y SVG"],
        en: ["Typography", "Symbol", "1 logo concept", "1 revision round", "Final files", "PNG, JPG, PDF and SVG"]
      }
    },
    {
      name: { es: "Logo Intermedio", en: "Intermediate Logo" },
      num: "02",
      usd: "$145", cop: "≈ $450.000 COP",
      list: {
        es: ["Investigación", "Idea / concepto", "Tipografía", "Símbolo", "2 propuestas de logo", "2 rondas de ajustes", "Archivos finales", "PNG, JPG, PDF y SVG"],
        en: ["Research", "Idea / concept", "Typography", "Symbol", "2 logo concepts", "2 revision rounds", "Final files", "PNG, JPG, PDF and SVG"]
      }
    },
    {
      name: { es: "Logo Avanzado", en: "Advanced Logo" },
      num: "03",
      usd: "$160", cop: "≈ $500.000 COP",
      badge: { es: "MÁS POPULAR", en: "MOST POPULAR" },
      list: {
        es: ["Investigación", "Idea / concepto", "Logo ilustrado", "3 propuestas de logo", "3 rondas de ajustes", "Versión blanco y negro", "Archivos finales profesionales", "PNG, JPG, PDF y SVG"],
        en: ["Research", "Idea / concept", "Illustrated logo", "3 logo concepts", "3 revision rounds", "Black & white version", "Professional final files", "PNG, JPG, PDF and SVG"]
      }
    }
  ];

  var PRICING_GUIDELINES = [
    {
      name: { es: "Basic Brand Guidelines", en: "Basic Brand Guidelines" },
      num: "01", usd: "$75", cop: "≈ $235.000 COP",
      list: {
        es: ["Variantes de logo", "Logometría", "Colorimetría HEX", "Tipografía", "1 mockup"],
        en: ["Logo variants", "Construction grid", "HEX colors", "Typography", "1 mockup"]
      }
    },
    {
      name: { es: "Intermediate Brand Guidelines", en: "Intermediate Brand Guidelines" },
      num: "02", usd: "$125", cop: "≈ $390.000 COP",
      list: {
        es: ["Presentación de marca", "Misión, visión y valores", "Variantes de logo", "Colorimetría HEX, RGB y CMYK", "Sistema gráfico", "5 mockups", "Aplicaciones para RRSS y web"],
        en: ["Brand presentation", "Mission, vision and values", "Logo variants", "HEX, RGB and CMYK colors", "Graphic system", "5 mockups", "Social media and web applications"]
      }
    },
    {
      name: { es: "Advanced Brand Guidelines", en: "Advanced Brand Guidelines" },
      num: "03", usd: "$200", cop: "≈ $628.000 COP",
      badge: { es: "RECOMENDADO", en: "RECOMMENDED" },
      list: {
        es: ["Presentación de marca", "Misión, visión y valores", "Personalidad y tono", "Target persona", "Usos correctos e incorrectos", "Colorimetría HEX, RGB y CMYK", "Sistema gráfico", "10 mockups", "Aplicaciones para RRSS y web"],
        en: ["Brand presentation", "Mission, vision and values", "Personality and tone", "Target persona", "Correct and incorrect usage", "HEX, RGB and CMYK colors", "Graphic system", "10 mockups", "Social media and web applications"]
      }
    }
  ];

  var PRICING_IDENTITY = [
    {
      name: { es: "Logo + Basic Visual Identity", en: "Logo + Basic Visual Identity" },
      num: "02", usd: "$250",
      list: {
        es: ["Logo principal y secundario", "Paleta de colores", "Tipografías", "Elementos gráficos básicos", "Imagen de perfil para redes sociales", "Hasta 3 rondas de modificaciones", "Archivos finales para digital e impresión"],
        en: ["Primary and secondary logo", "Color palette", "Typography", "Basic graphic elements", "Profile image for social media", "Up to 3 revision rounds", "Final files for digital and print"]
      }
    },
    {
      name: { es: "Brand Identity", en: "Brand Identity" },
      num: "03", usd: "$450",
      list: {
        es: ["Concepto visual de marca", "Logo principal y secundario", "Isotipo o símbolo", "Variaciones del logo", "Paleta de colores y sistema tipográfico", "Guía de identidad visual", "Archivos finales para digital e impresión"],
        en: ["Brand visual concept", "Primary and secondary logo", "Isotype or symbol", "Logo variations", "Color palette and typography system", "Visual identity guide", "Final files for digital and print"]
      }
    },
    {
      name: { es: "Complete Branding", en: "Complete Branding" },
      num: "04", usd: "$650",
      list: {
        es: ["Identidad de marca completa", "Manual profesional de marca", "Portada para Facebook", "5 plantillas para redes sociales", "Tarjeta de presentación", "Papelería básica", "Archivos editables y finales"],
        en: ["Complete brand identity", "Professional brand manual", "Facebook cover", "5 social media templates", "Business card", "Basic stationery", "Editable and final files"]
      }
    }
  ];

  var PRICING_SOCIAL = [
    { name: { es: "Portada Facebook", en: "Facebook Cover" }, usd: "$40" },
    { name: { es: "Pieza individual", en: "Individual Graphic" }, usd: "$25" },
    { name: { es: "5 piezas", en: "5 Graphics" }, usd: "$100" },
    { name: { es: "10 piezas", en: "10 Graphics" }, usd: "$180" }
  ];

  /* =====================================================
     WHY TAKOI
  ===================================================== */
  var WHY = [
    { es: "Diseño personalizado", en: "Custom design" },
    { es: "Proceso estratégico", en: "Strategic process" },
    { es: "Comunicación directa", en: "Direct communication" },
    { es: "Archivos profesionales", en: "Professional final files" },
    { es: "Trabajo remoto", en: "Remote collaboration" },
    { es: "Atención personalizada", en: "Personalized service" },
    { es: "Diseño para digital e impresión", en: "Digital and print ready" }
  ];

  /* =====================================================
     FAQ
  ===================================================== */
  var FAQ = [
    {
      q: { es: "¿Cuántas modificaciones incluye cada paquete?", en: "How many revisions does each package include?" },
      a: {
        es: "Depende del paquete: cada uno especifica el número exacto de rondas de ajustes incluidas, desde 1 hasta 3. Cambios adicionales o sustanciales pueden generar un costo extra.",
        en: "It depends on the package: each one specifies the exact number of revision rounds included, from 1 to 3. Additional or substantial changes may incur an extra cost."
      }
    },
    {
      q: { es: "¿Trabajas con clientes fuera de Colombia?", en: "Do you work with clients outside Colombia?" },
      a: {
        es: "Sí. Trabajo de forma remota con clientes en Estados Unidos, Florida y otros países, coordinando todo por WhatsApp y correo electrónico.",
        en: "Yes. I work remotely with clients in the United States, Florida and other countries, coordinating everything over WhatsApp and email."
      }
    },
    {
      q: { es: "¿Cómo funciona el proceso?", en: "How does the process work?" },
      a: {
        es: "Completas el brief interactivo, revisamos juntos tu proyecto, te presento propuestas según el paquete elegido y avanzamos por las rondas de ajustes hasta la entrega final.",
        en: "You complete the interactive brief, we review your project together, I present concepts based on the chosen package, and we move through the revision rounds until final delivery."
      }
    },
    {
      q: { es: "¿Qué archivos recibiré?", en: "What files will I receive?" },
      a: {
        es: "Normalmente PNG, JPG, PDF y SVG para uso digital e impresión. Los archivos editables dependen del paquete contratado.",
        en: "Typically PNG, JPG, PDF and SVG for digital and print use. Editable files depend on the package you choose."
      }
    },
    {
      q: { es: "¿Los archivos editables están incluidos?", en: "Are editable files included?" },
      a: {
        es: "Solo en los paquetes que lo indican explícitamente, como Complete Branding. Si necesitas archivos editables en otro paquete, lo podemos conversar.",
        en: "Only in the packages that explicitly state it, like Complete Branding. If you need editable files in another package, we can discuss it."
      }
    },
    {
      q: { es: "¿Cuánto tiempo toma un proyecto?", en: "How long does a project take?" },
      a: {
        es: "Varía según el paquete y la cantidad de rondas de ajustes, pero se coordina un cronograma claro desde el inicio del proyecto.",
        en: "It varies depending on the package and the number of revision rounds, but a clear timeline is agreed at the start of the project."
      }
    },
    {
      q: { es: "¿Cómo se realiza el pago?", en: "How is payment handled?" },
      a: {
        es: "50% de anticipo para iniciar el proyecto y 50% restante al finalizar, antes de la entrega de los archivos editables cuando estén incluidos.",
        en: "50% deposit to start the project and the remaining 50% upon completion, before delivery of editable files when included."
      }
    }
  ];

  /* =====================================================
     WIZARD — service options & step templates
  ===================================================== */
  var SERVICE_OPTIONS = [
    { key: "logo-basico", group: "default", es: "Logo Básico", en: "Basic Logo" },
    { key: "logo-intermedio", group: "default", es: "Logo Intermedio", en: "Intermediate Logo" },
    { key: "logo-avanzado", group: "default", es: "Logo Avanzado", en: "Advanced Logo" },
    { key: "logo-identity", group: "default", es: "Logo + Identidad Visual", en: "Logo + Visual Identity" },
    { key: "brand-identity", group: "default", es: "Brand Identity", en: "Brand Identity" },
    { key: "complete-branding", group: "default", es: "Complete Branding", en: "Complete Branding" },
    { key: "brand-guidelines", group: "guidelines", es: "Brand Guidelines", en: "Brand Guidelines" },
    { key: "social-media", group: "social", es: "Social Media Design", en: "Social Media Design" },
    { key: "other", group: "default", es: "Otro", en: "Other" }
  ];

  var OBJECTIVE_OPTIONS = [
    { es: "Dar a conocer mi negocio", en: "Raise awareness of my business" },
    { es: "Conseguir más clientes", en: "Get more clients" },
    { es: "Lanzar un nuevo proyecto", en: "Launch a new project" },
    { es: "Renovar mi imagen", en: "Refresh my image" },
    { es: "Diferenciarme de la competencia", en: "Stand out from competitors" },
    { es: "Profesionalizar mi marca", en: "Make my brand more professional" },
    { es: "Otro", en: "Other" }
  ];

  var FEELING_OPTIONS = [
    { es: "Confianza", en: "Trust" }, { es: "Profesionalismo", en: "Professionalism" },
    { es: "Elegancia", en: "Elegance" }, { es: "Cercanía", en: "Warmth" },
    { es: "Creatividad", en: "Creativity" }, { es: "Innovación", en: "Innovation" },
    { es: "Exclusividad", en: "Exclusivity" }, { es: "Diversión", en: "Fun" },
    { es: "Seguridad", en: "Security" }, { es: "Modernidad", en: "Modernity" }
  ];

  var STYLE_OPTIONS = [
    { es: "Minimalista", en: "Minimalist" }, { es: "Moderna", en: "Modern" },
    { es: "Elegante", en: "Elegant" }, { es: "Premium", en: "Premium" },
    { es: "Creativa", en: "Creative" }, { es: "Corporativa", en: "Corporate" },
    { es: "Divertida", en: "Fun" }, { es: "Sofisticada", en: "Sophisticated" },
    { es: "Orgánica", en: "Organic" }, { es: "Juvenil", en: "Youthful" },
    { es: "Femenina", en: "Feminine" }, { es: "Masculina", en: "Masculine" },
    { es: "Artesanal", en: "Handcrafted" }, { es: "Tecnológica", en: "Tech" }
  ];

  var PLACEMENT_OPTIONS = [
    { es: "Instagram", en: "Instagram" }, { es: "Facebook", en: "Facebook" },
    { es: "TikTok", en: "TikTok" }, { es: "Website", en: "Website" },
    { es: "Packaging", en: "Packaging" }, { es: "Impresos", en: "Print" },
    { es: "Publicidad", en: "Advertising" }, { es: "Otro", en: "Other" }
  ];

  // Step templates: array of {key, title, subtitle, fields:[...]}
  // field.type: text | email | tel | url | textarea | chips (single) | chips-multi
  function buildSteps(group) {
    var steps = [];

    steps.push({
      key: "about-you",
      title: { es: "Sobre ti", en: "About you" },
      subtitle: { es: "Para poder contactarte.", en: "So we can get in touch." },
      fields: [
        { id: "name", type: "text", required: true, label: { es: "Nombre / Empresa", en: "Name / Company" } },
        { id: "email", type: "email", required: true, label: { es: "Email", en: "Email" } },
        { id: "phone", type: "tel", required: true, label: { es: "WhatsApp / Teléfono", en: "WhatsApp / Phone" } },
        { id: "website", type: "url", required: false, label: { es: "Sitio web (opcional)", en: "Website (optional)" } },
        { id: "social", type: "text", required: false, label: { es: "Instagram / Redes sociales (opcional)", en: "Instagram / Social media (optional)" } }
      ]
    });

    if (group === "social") {
      steps.push({
        key: "about-brand",
        title: { es: "Sobre tu marca", en: "About your brand" },
        subtitle: { es: "Un poco de contexto sobre tu negocio.", en: "A little context about your business." },
        fields: [
          { id: "brandName", type: "text", required: true, label: { es: "¿Cuál es el nombre exacto de la marca?", en: "What's the exact name of the brand?" } },
          { id: "brandWhat", type: "textarea", required: true, label: { es: "¿A qué se dedica tu marca?", en: "What does your brand do?" } },
          { id: "hasGuidelines", type: "chips", required: false, label: { es: "¿Ya tienes colores y tipografía definidos?", en: "Do you already have defined colors and typography?" }, options: [{ es: "Sí", en: "Yes" }, { es: "No", en: "No" }, { es: "Parcialmente", en: "Partially" }] }
        ]
      });
      steps.push({
        key: "content",
        title: { es: "Sobre tu contenido", en: "About your content" },
        subtitle: { es: "Para entender qué necesitas publicar.", en: "So we understand what you need to publish." },
        fields: [
          { id: "contentType", type: "textarea", required: true, label: { es: "¿Qué tipo de contenido publicas normalmente?", en: "What kind of content do you usually post?" } },
          { id: "quantity", type: "chips", required: true, label: { es: "¿Cuántas piezas necesitas?", en: "How many pieces do you need?" }, options: [{ es: "Portada Facebook", en: "Facebook cover" }, { es: "Pieza individual", en: "Individual graphic" }, { es: "5 piezas", en: "5 graphics" }, { es: "10 piezas", en: "10 graphics" }] },
          { id: "feeling", type: "chips-multi", required: false, label: { es: "¿Qué quieres que sienta tu audiencia?", en: "What do you want your audience to feel?" }, options: FEELING_OPTIONS }
        ]
      });
      steps.push({
        key: "references",
        title: { es: "Referencias", en: "References" },
        subtitle: { es: "Marcas o estilos que te gustan.", en: "Brands or styles you like." },
        fields: [
          { id: "likedBrands", type: "textarea", required: false, label: { es: "¿Qué marcas o cuentas te gustan visualmente?", en: "What brands or accounts do you like visually?" } },
          { id: "avoid", type: "textarea", required: false, label: { es: "¿Hay algo que definitivamente no quieres?", en: "Is there anything you definitely don't want?" } }
        ]
      });
      steps.push({
        key: "project-details",
        title: { es: "Detalles del proyecto", en: "Project details" },
        subtitle: { es: "Últimos detalles antes de enviar.", en: "A few last details before sending." },
        fields: [
          { id: "deadline", type: "text", required: false, label: { es: "¿Tienes alguna fecha límite?", en: "Do you have a deadline?" } },
          { id: "extra", type: "textarea", required: false, label: { es: "¿Hay algo más que quieras contarnos sobre tu proyecto?", en: "Anything else you'd like to tell us about your project?" } }
        ]
      });
    } else if (group === "guidelines") {
      steps.push({
        key: "about-brand",
        title: { es: "Sobre tu marca", en: "About your brand" },
        subtitle: { es: "Para preparar tu manual de marca.", en: "To prepare your brand manual." },
        fields: [
          { id: "brandName", type: "text", required: true, label: { es: "¿Cuál es el nombre exacto de la marca?", en: "What's the exact name of the brand?" } },
          { id: "brandWhat", type: "textarea", required: true, label: { es: "¿A qué se dedica tu marca?", en: "What does your brand do?" } },
          { id: "hasLogo", type: "chips", required: true, label: { es: "¿Ya tienes un logo definido?", en: "Do you already have a defined logo?" }, options: [{ es: "Sí", en: "Yes" }, { es: "No", en: "No" }] },
          { id: "objective", type: "chips", required: true, label: { es: "¿Por qué necesitas un manual de marca ahora?", en: "Why do you need a brand manual now?" }, options: OBJECTIVE_OPTIONS }
        ]
      });
      steps.push({
        key: "audience",
        title: { es: "Tu audiencia", en: "Your audience" },
        subtitle: { es: "Para alinear el tono del manual.", en: "To align the manual's tone." },
        fields: [
          { id: "idealClient", type: "textarea", required: false, label: { es: "¿Quién es tu cliente ideal?", en: "Who is your ideal customer?" } },
          { id: "feeling", type: "chips-multi", required: false, label: { es: "¿Qué quieres que tu cliente sienta al ver tu marca?", en: "What do you want your customer to feel when they see your brand?" }, options: FEELING_OPTIONS }
        ]
      });
      steps.push({
        key: "manual-scope",
        title: { es: "Contenido del manual", en: "Manual contents" },
        subtitle: { es: "Qué necesitas que incluya.", en: "What you need it to include." },
        fields: [
          { id: "elements", type: "textarea", required: false, label: { es: "¿Qué elementos necesitas incluir en el manual?", en: "What elements do you need included in the manual?" } },
          { id: "usage", type: "text", required: false, label: { es: "¿Para qué usarán el manual? (equipo interno, imprenta, redes...)", en: "What will the manual be used for? (internal team, print shop, social media...)" } }
        ]
      });
      steps.push({
        key: "references",
        title: { es: "Referencias", en: "References" },
        subtitle: { es: "Manuales o marcas que te gustan.", en: "Manuals or brands you like." },
        fields: [
          { id: "likedBrands", type: "textarea", required: false, label: { es: "¿Qué marcas te gustan visualmente?", en: "What brands do you like visually?" } },
          { id: "competitors", type: "text", required: false, label: { es: "¿Quiénes son tus principales competidores?", en: "Who are your main competitors?" } }
        ]
      });
      steps.push({
        key: "project-details",
        title: { es: "Detalles del proyecto", en: "Project details" },
        subtitle: { es: "Últimos detalles antes de enviar.", en: "A few last details before sending." },
        fields: [
          { id: "deadline", type: "text", required: false, label: { es: "¿Tienes alguna fecha límite?", en: "Do you have a deadline?" } },
          { id: "extra", type: "textarea", required: false, label: { es: "¿Hay algo más que quieras contarnos sobre tu proyecto?", en: "Anything else you'd like to tell us about your project?" } }
        ]
      });
    } else {
      // default: logo tiers, logo+identity, brand identity, complete branding, other
      steps.push({
        key: "about-brand",
        title: { es: "Sobre tu marca", en: "About your brand" },
        subtitle: { es: "Cuéntame quién eres.", en: "Tell me who you are." },
        fields: [
          { id: "brandName", type: "text", required: true, label: { es: "¿Cuál es el nombre exacto de la marca?", en: "What's the exact name of the brand?" } },
          { id: "brandWhat", type: "textarea", required: true, label: { es: "¿A qué se dedica tu marca?", en: "What does your brand do?" } },
          { id: "origin", type: "textarea", required: false, label: { es: "¿Cómo nació tu proyecto?", en: "How did your project start?" } },
          { id: "objective", type: "chips", required: true, label: { es: "¿Cuál es el principal objetivo de tu marca?", en: "What is your brand's main objective?" }, options: OBJECTIVE_OPTIONS },
          { id: "different", type: "textarea", required: false, label: { es: "¿Qué hace diferente a tu marca?", en: "What makes your brand different?" } }
        ]
      });
      steps.push({
        key: "audience",
        title: { es: "Tu audiencia", en: "Your audience" },
        subtitle: { es: "Para quién estamos diseñando.", en: "Who we're designing for." },
        fields: [
          { id: "idealClient", type: "textarea", required: false, label: { es: "¿Quién es tu cliente ideal?", en: "Who is your ideal customer?" } },
          { id: "feeling", type: "chips-multi", required: false, label: { es: "¿Qué quieres que tu cliente sienta cuando vea tu marca?", en: "What do you want your customer to feel when they see your brand?" }, options: FEELING_OPTIONS },
          { id: "perception", type: "text", required: false, label: { es: "¿Cómo quieres que tu marca sea percibida?", en: "How do you want your brand to be perceived?" } }
        ]
      });
      steps.push({
        key: "visual",
        title: { es: "Dirección visual", en: "Visual direction" },
        subtitle: { es: "Cómo imaginas tu marca.", en: "How you imagine your brand." },
        fields: [
          { id: "style", type: "chips-multi", required: false, label: { es: "¿Cómo imaginas visualmente tu marca?", en: "How do you visually imagine your brand?" }, options: STYLE_OPTIONS },
          { id: "colorsWant", type: "text", required: false, label: { es: "¿Qué colores te gustaría utilizar?", en: "What colors would you like to use?" } },
          { id: "colorsAvoid", type: "text", required: false, label: { es: "¿Qué colores NO quieres utilizar?", en: "What colors do you NOT want to use?" } },
          { id: "symbol", type: "text", required: false, label: { es: "¿Hay algún símbolo o elemento que quieras incorporar?", en: "Is there a symbol or element you'd like to include?" } },
          { id: "avoid", type: "text", required: false, label: { es: "¿Hay algo que definitivamente NO quieres?", en: "Is there anything you definitely don't want?" } }
        ]
      });
      steps.push({
        key: "references",
        title: { es: "Referencias", en: "References" },
        subtitle: { es: "Marcas que admiras y competencia.", en: "Brands you admire and your competitors." },
        fields: [
          { id: "likedBrands", type: "textarea", required: false, label: { es: "¿Qué marcas te gustan visualmente y qué te gusta de ellas?", en: "What brands do you like visually, and what do you like about them?" } },
          { id: "competitors", type: "text", required: false, label: { es: "¿Quiénes son tus principales competidores?", en: "Who are your main competitors?" } },
          { id: "differentiation", type: "text", required: false, label: { es: "¿Cómo quieres diferenciarte de ellos?", en: "How do you want to stand out from them?" } }
        ]
      });
      steps.push({
        key: "project-details",
        title: { es: "Detalles del proyecto", en: "Project details" },
        subtitle: { es: "Últimos detalles antes de enviar.", en: "A few last details before sending." },
        fields: [
          { id: "placement", type: "chips-multi", required: false, label: { es: "¿Dónde utilizarás principalmente el diseño?", en: "Where will you mainly use the design?" }, options: PLACEMENT_OPTIONS },
          { id: "deadline", type: "text", required: false, label: { es: "¿Tienes alguna fecha límite?", en: "Do you have a deadline?" } },
          { id: "requirements", type: "text", required: false, label: { es: "¿Hay algún requisito técnico?", en: "Any technical requirements?" } },
          { id: "extra", type: "textarea", required: false, label: { es: "¿Hay algo más que quieras contarnos sobre tu proyecto?", en: "Anything else you'd like to tell us about your project?" } }
        ]
      });
    }

    return steps;
  }

  /* =====================================================
     RENDER: static i18n text
  ===================================================== */
  function applyStaticI18n() {
    document.documentElement.lang = state.lang;
    document.documentElement.setAttribute("data-lang", state.lang);
    document.querySelectorAll("[data-i18n]").forEach(function (el) {
      el.textContent = t(el.getAttribute("data-i18n"));
    });
    document.querySelectorAll(".lang-btn").forEach(function (b) {
      b.classList.toggle("active", b.getAttribute("data-lang-btn") === state.lang);
    });
  }

  /* =====================================================
     RENDER: services modal open
  ===================================================== */
  function openServiceModal(key) {
    var d = SERVICE_DETAILS[key];
    if (!d) return;
    document.getElementById("modalTitle").textContent = L(d.title);
    document.getElementById("modalText").textContent = L(d.text);
    var ul = document.getElementById("modalList");
    ul.innerHTML = "";
    L(d.list).forEach(function (item) {
      var li = document.createElement("li");
      li.textContent = item;
      ul.appendChild(li);
    });
    openOverlay("serviceModalOverlay");
  }

  function openInfoModal(title, text, list) {
    document.getElementById("modalTitle").textContent = title;
    document.getElementById("modalText").textContent = text;
    var ul = document.getElementById("modalList");
    ul.innerHTML = "";
    list.forEach(function (item) {
      var li = document.createElement("li");
      li.textContent = item;
      ul.appendChild(li);
    });
    openOverlay("serviceModalOverlay");
  }

  function openProjectModal(item) {
    document.getElementById("projectModalImg").src = item.img;
    document.getElementById("projectModalImg").alt = L(item.name);
    document.getElementById("projectModalTitle").textContent = L(item.name);
    document.getElementById("projectModalText").textContent = L(item.desc);
    var link = document.getElementById("projectModalLink");
    link.href = item.pdf;
    withFallback(document.getElementById("projectModalImg"));
    openOverlay("projectModalOverlay");
  }

  function openOverlay(id) {
    document.getElementById(id).classList.add("open");
    document.body.style.overflow = "hidden";
  }
  function closeOverlay(id) {
    document.getElementById(id).classList.remove("open");
    document.body.style.overflow = "";
  }

  /* =====================================================
     RENDER: logo grid
  ===================================================== */
  function renderLogoGrid() {
    var grid = document.getElementById("logoGrid");
    grid.innerHTML = "";
    LOGOS.forEach(function (item) {
      var card = document.createElement("div");
      card.className = "logo-card reveal";
      if (state.filter !== "all" && item.cat !== state.filter) card.classList.add("hidden");
      var catLabel = L(FILTER_LABELS[item.cat]);
      card.innerHTML =
        '<div class="logo-img-box"><img alt="' + L(item.name) + '"></div>' +
        '<div class="logo-card-info"><h4>' + L(item.name) + "</h4><span>" + L(item.client) + " · " + catLabel + "</span></div>" +
        '<button type="button" class="logo-card-btn">' + t("services.more") + "</button>";
      var img = card.querySelector("img");
      img.src = item.img;
      withFallback(img);
      card.querySelector(".logo-card-btn").addEventListener("click", function () {
        openInfoModal(L(item.name), L(item.client) + " — " + catLabel, []);
      });
      grid.appendChild(card);
    });
    observeReveal();
  }

  /* =====================================================
     RENDER: brand identity editorial
  ===================================================== */
  function renderBrandEditorial() {
    var grid = document.getElementById("brandEditorialGrid");
    grid.innerHTML = "";
    BRAND_EDITORIAL.forEach(function (item) {
      var card = document.createElement("div");
      card.className = "brand-editorial-card reveal";
      card.innerHTML =
        '<div class="img-box"><img alt="' + L(item.name) + '"></div>' +
        '<div class="card-body"><span class="cat-tag">' + L(item.cat) + "</span>" +
        "<h3>" + L(item.name) + "</h3><p>" + L(item.desc) + "</p>" +
        '<button type="button">' + t("modal.viewpdf") + "</button></div>";
      var img = card.querySelector("img");
      img.src = item.img;
      withFallback(img);
      card.querySelector("button").addEventListener("click", function () {
        openProjectModal(item);
      });
      grid.appendChild(card);
    });
    observeReveal();
  }

  /* =====================================================
     RENDER: pricing
  ===================================================== */
  function priceCardHTML(item) {
    var badge = item.badge ? '<span class="price-badge">' + L(item.badge) + "</span>" : "";
    var popularClass = item.badge ? " popular" : "";
    var copLine = item.cop ? '<span class="price-cop">' + item.cop + "</span>" : "";
    return (
      '<div class="price-card' + popularClass + ' reveal">' +
      badge +
      (item.num ? '<span style="font-size:.72rem;font-weight:700;color:var(--ink-soft);">' + item.num + "</span>" : "") +
      "<h4>" + L(item.name) + "</h4>" +
      '<span class="price-usd">' + item.usd + "</span>" +
      copLine +
      "</div>"
    );
  }

  function renderPricing() {
    var logoWrap = document.getElementById("pricingLogos");
    logoWrap.innerHTML = "";
    PRICING_LOGOS.forEach(function (item) {
      var div = document.createElement("div");
      div.innerHTML = priceCardHTML(item);
      var card = div.firstChild;
      card.addEventListener("click", function () {
        openInfoModal(L(item.name) + " — " + item.usd, item.cop || "", L(item.list));
      });
      logoWrap.appendChild(card);
    });

    var guideWrap = document.getElementById("pricingGuidelines");
    guideWrap.innerHTML = "";
    PRICING_GUIDELINES.forEach(function (item) {
      var div = document.createElement("div");
      div.innerHTML = priceCardHTML(item);
      var card = div.firstChild;
      card.addEventListener("click", function () {
        openInfoModal(L(item.name) + " — " + item.usd, item.cop || "", L(item.list));
      });
      guideWrap.appendChild(card);
    });

    var identityWrap = document.getElementById("pricingIdentity");
    identityWrap.innerHTML = "";
    PRICING_IDENTITY.forEach(function (item) {
      var div = document.createElement("div");
      div.innerHTML = priceCardHTML(item);
      var card = div.firstChild;
      card.addEventListener("click", function () {
        openInfoModal(L(item.name) + " — " + item.usd, "", L(item.list));
      });
      identityWrap.appendChild(card);
    });

    var socialWrap = document.getElementById("pricingSocial");
    socialWrap.innerHTML = "";
    var deliveredNote = { es: "Archivos finales incluidos", en: "Final files included" };
    PRICING_SOCIAL.forEach(function (item) {
      var card = document.createElement("div");
      card.className = "social-price-card reveal";
      card.innerHTML =
        "<h4>" + L(item.name) + '</h4><span class="price-usd">' + item.usd + "</span>" +
        '<div style="font-size:.72rem;color:var(--ink-soft);margin-top:8px;">' + L(deliveredNote) + "</div>";
      socialWrap.appendChild(card);
    });

    observeReveal();
  }

  /* =====================================================
     RENDER: why + faq
  ===================================================== */
  var CHECK_ICON =
    '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><circle cx="12" cy="12" r="9"></circle><path d="m8 12.5 2.5 2.5L16 9.5"></path></svg>';

  function renderWhy() {
    var grid = document.getElementById("whyGrid");
    grid.innerHTML = "";
    WHY.forEach(function (item) {
      var div = document.createElement("div");
      div.className = "why-item reveal";
      div.innerHTML = CHECK_ICON + "<p>" + L(item) + "</p>";
      grid.appendChild(div);
    });
    observeReveal();
  }

  function renderFaq() {
    var wrap = document.getElementById("faqAccordion");
    wrap.innerHTML = "";
    FAQ.forEach(function (item, i) {
      var el = document.createElement("div");
      el.className = "accordion-item";
      el.innerHTML =
        '<button type="button" class="accordion-trigger" aria-expanded="false">' +
        "<span>" + L(item.q) + '</span><span class="plus">+</span></button>' +
        '<div class="accordion-panel"><p>' + L(item.a) + "</p></div>";
      var trigger = el.querySelector(".accordion-trigger");
      var panel = el.querySelector(".accordion-panel");
      trigger.addEventListener("click", function () {
        var isOpen = el.classList.contains("open");
        wrap.querySelectorAll(".accordion-item.open").forEach(function (openEl) {
          openEl.classList.remove("open");
          openEl.querySelector(".accordion-trigger").setAttribute("aria-expanded", "false");
          openEl.querySelector(".accordion-panel").style.maxHeight = null;
        });
        if (!isOpen) {
          el.classList.add("open");
          trigger.setAttribute("aria-expanded", "true");
          panel.style.maxHeight = panel.scrollHeight + "px";
        }
      });
      wrap.appendChild(el);
    });
  }

  /* =====================================================
     WIZARD LOGIC
  ===================================================== */
  var wizard = {
    serviceKey: null,
    group: null,
    steps: [],
    stepIndex: 0, // 0 = service select
    answers: {}
  };

  function totalWizardSteps() {
    // service-select + N content steps + review
    return wizard.steps.length + 2;
  }

  function renderWizardStep() {
    var container = document.getElementById("wizardSteps");
    container.innerHTML = "";
    var backBtn = document.getElementById("backBtn");
    var nextBtn = document.getElementById("nextBtn");
    var submitBtn = document.getElementById("submitBtn");
    backBtn.hidden = wizard.stepIndex === 0;
    submitBtn.hidden = true;
    nextBtn.hidden = false;

    var total = totalWizardSteps();
    var progressPct = (wizard.stepIndex / (total - 1)) * 100;
    document.getElementById("progressFill").style.width = progressPct + "%";
    var stepLabelTpl = state.lang === "es" ? "Paso " + (wizard.stepIndex + 1) + " de " + total : "Step " + (wizard.stepIndex + 1) + " of " + total;
    document.getElementById("stepLabel").textContent = stepLabelTpl;

    var stepEl = document.createElement("div");
    stepEl.className = "wizard-step";

    if (wizard.stepIndex === 0) {
      stepEl.innerHTML =
        "<h3>" + (state.lang === "es" ? "¿Qué servicio te interesa?" : "Which service are you interested in?") + "</h3>" +
        '<p class="step-sub">' + (state.lang === "es" ? "Así puedo mostrarte las preguntas más relevantes." : "This lets us show you the most relevant questions.") + "</p>" +
        '<div class="service-select-grid" id="serviceSelectGrid"></div>';
      container.appendChild(stepEl);
      var grid = stepEl.querySelector("#serviceSelectGrid");
      SERVICE_OPTIONS.forEach(function (opt) {
        var btn = document.createElement("button");
        btn.type = "button";
        btn.className = "service-select-card" + (wizard.serviceKey === opt.key ? " selected" : "");
        btn.textContent = opt[state.lang];
        btn.addEventListener("click", function () {
          wizard.serviceKey = opt.key;
          wizard.group = opt.group;
          wizard.steps = buildSteps(opt.group);
          grid.querySelectorAll(".service-select-card").forEach(function (c) {
            c.classList.remove("selected");
          });
          btn.classList.add("selected");
        });
        grid.appendChild(btn);
      });
    } else if (wizard.stepIndex <= wizard.steps.length) {
      var stepDef = wizard.steps[wizard.stepIndex - 1];
      stepEl.innerHTML =
        "<h3>" + L(stepDef.title) + '</h3><p class="step-sub">' + L(stepDef.subtitle) + "</p>";
      stepDef.fields.forEach(function (f) {
        stepEl.appendChild(renderField(f));
      });
      container.appendChild(stepEl);
    } else {
      // review step
      stepEl.innerHTML =
        "<h3>" + (state.lang === "es" ? "Resumen de tu brief" : "Your brief summary") + '</h3><p class="step-sub">' +
        (state.lang === "es" ? "Revisa la información antes de enviarla." : "Review the information before sending it.") + "</p>";
      var dl = document.createElement("dl");
      dl.className = "summary-list";
      var serviceOpt = SERVICE_OPTIONS.filter(function (o) { return o.key === wizard.serviceKey; })[0];
      addSummaryRow(dl, state.lang === "es" ? "Servicio" : "Service", serviceOpt ? serviceOpt[state.lang] : "—");
      Object.keys(wizard.answers).forEach(function (key) {
        var val = wizard.answers[key];
        if (!val || (Array.isArray(val) && val.length === 0)) return;
        addSummaryRow(dl, fieldLabelById(key), Array.isArray(val) ? val.join(", ") : val);
      });
      stepEl.appendChild(dl);
      container.appendChild(stepEl);
      nextBtn.hidden = true;
      submitBtn.hidden = false;
    }
  }

  function fieldLabelById(id) {
    var found = null;
    wizard.steps.forEach(function (s) {
      s.fields.forEach(function (f) {
        if (f.id === id) found = f;
      });
    });
    return found ? L(found.label) : id;
  }

  function addSummaryRow(dl, label, value) {
    var row = document.createElement("div");
    row.className = "summary-row";
    row.innerHTML = "<dt>" + label + "</dt><dd></dd>";
    row.querySelector("dd").textContent = value;
    dl.appendChild(row);
  }

  function renderField(f) {
    var wrap = document.createElement("div");
    wrap.className = "field";
    wrap.setAttribute("data-field-id", f.id);
    var label = document.createElement("label");
    label.textContent = L(f.label) + (f.required ? " *" : "");
    wrap.appendChild(label);

    if (f.type === "textarea") {
      var ta = document.createElement("textarea");
      ta.value = wizard.answers[f.id] || "";
      ta.addEventListener("input", function () {
        wizard.answers[f.id] = ta.value;
        clearFieldError(wrap);
      });
      wrap.appendChild(ta);
    } else if (f.type === "chips") {
      var chipGrid = document.createElement("div");
      chipGrid.className = "option-grid";
      f.options.forEach(function (opt) {
        var chip = document.createElement("button");
        chip.type = "button";
        chip.className = "option-chip" + (wizard.answers[f.id] === L(opt) ? " selected" : "");
        chip.textContent = L(opt);
        chip.addEventListener("click", function () {
          wizard.answers[f.id] = L(opt);
          chipGrid.querySelectorAll(".option-chip").forEach(function (c) { c.classList.remove("selected"); });
          chip.classList.add("selected");
          clearFieldError(wrap);
        });
        chipGrid.appendChild(chip);
      });
      wrap.appendChild(chipGrid);
    } else if (f.type === "chips-multi") {
      var chipGridM = document.createElement("div");
      chipGridM.className = "option-grid";
      var current = wizard.answers[f.id] || [];
      f.options.forEach(function (opt) {
        var chip = document.createElement("button");
        chip.type = "button";
        var label2 = L(opt);
        chip.className = "option-chip" + (current.indexOf(label2) > -1 ? " selected" : "");
        chip.textContent = label2;
        chip.addEventListener("click", function () {
          var arr = wizard.answers[f.id] || [];
          var idx = arr.indexOf(label2);
          if (idx > -1) { arr.splice(idx, 1); chip.classList.remove("selected"); }
          else { arr.push(label2); chip.classList.add("selected"); }
          wizard.answers[f.id] = arr;
        });
        chipGridM.appendChild(chip);
      });
      wrap.appendChild(chipGridM);
    } else {
      var input = document.createElement("input");
      input.type = f.type;
      input.value = wizard.answers[f.id] || "";
      input.addEventListener("input", function () {
        wizard.answers[f.id] = input.value;
        clearFieldError(wrap);
      });
      wrap.appendChild(input);
    }

    var errMsg = document.createElement("div");
    errMsg.className = "field-error-msg";
    errMsg.textContent = state.lang === "es" ? "Este campo es obligatorio." : "This field is required.";
    wrap.appendChild(errMsg);
    return wrap;
  }

  function clearFieldError(wrap) {
    wrap.classList.remove("error");
  }

  function validateCurrentStep() {
    if (wizard.stepIndex === 0) {
      if (!wizard.serviceKey) {
        return false;
      }
      return true;
    }
    if (wizard.stepIndex > wizard.steps.length) return true; // review step

    var stepDef = wizard.steps[wizard.stepIndex - 1];
    var valid = true;
    stepDef.fields.forEach(function (f) {
      if (!f.required) return;
      var val = wizard.answers[f.id];
      var empty = !val || (Array.isArray(val) && val.length === 0) || (typeof val === "string" && val.trim() === "");
      var fieldWrap = document.querySelector('[data-field-id="' + f.id + '"]');
      if (empty) {
        valid = false;
        if (fieldWrap) fieldWrap.classList.add("error");
      } else if (f.type === "email" && !/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(val)) {
        valid = false;
        if (fieldWrap) {
          fieldWrap.classList.add("error");
          fieldWrap.querySelector(".field-error-msg").textContent =
            state.lang === "es" ? "Ingresa un email válido." : "Enter a valid email.";
        }
      }
    });
    return valid;
  }

  function initWizard() {
    wizard.serviceKey = null;
    wizard.group = null;
    wizard.steps = [];
    wizard.stepIndex = 0;
    wizard.answers = {};
    document.getElementById("briefForm").hidden = false;
    document.getElementById("wizardSuccess").hidden = true;
    renderWizardStep();
  }

  // ============================================================
  // DEMO SUBMIT FUNCTION — CONECTA AQUÍ TU BACKEND REAL
  // Reemplaza el cuerpo de esta función por una llamada real a
  // Formspree, Netlify Forms o EmailJS. Ejemplo con Formspree:
  //
  //   return fetch('https://formspree.io/f/TU_ID_AQUI', {
  //     method: 'POST',
  //     headers: { 'Content-Type': 'application/json', Accept: 'application/json' },
  //     body: JSON.stringify(payload)
  //   }).then(function(res){ return { ok: res.ok }; });
  //
  // ============================================================
  function submitBriefToBackend(payload) {
    console.log("Brief recibido (demo — aún no conectado a un backend real):", payload);
    return new Promise(function (resolve) {
      setTimeout(function () {
        resolve({ ok: true });
      }, 700);
    });
  }

  function handleWizardSubmit(e) {
    e.preventDefault();
    var submitBtn = document.getElementById("submitBtn");
    submitBtn.disabled = true;
    var originalText = submitBtn.textContent;
    submitBtn.textContent = state.lang === "es" ? "Enviando..." : "Sending...";

    var payload = {
      service: wizard.serviceKey,
      answers: wizard.answers,
      lang: state.lang,
      submittedAt: new Date().toISOString()
    };

    submitBriefToBackend(payload).then(function (result) {
      submitBtn.disabled = false;
      submitBtn.textContent = originalText;
      if (result && result.ok) {
        document.getElementById("briefForm").hidden = true;
        document.getElementById("wizardSuccess").hidden = false;
      }
    });
  }

  /* =====================================================
     SCROLL REVEAL
  ===================================================== */
  var revealObserver;
  function observeReveal() {
    if (!("IntersectionObserver" in window)) return;
    if (!revealObserver) {
      revealObserver = new IntersectionObserver(
        function (entries) {
          entries.forEach(function (entry) {
            if (entry.isIntersecting) {
              entry.target.classList.add("in-view");
              revealObserver.unobserve(entry.target);
            }
          });
        },
        { threshold: 0.08, rootMargin: "0px 0px -40px 0px" }
      );
    }
    document.querySelectorAll(".reveal:not(.in-view)").forEach(function (el) {
      revealObserver.observe(el);
    });
  }

  /* =====================================================
     FULL RENDER (called on init + language switch)
  ===================================================== */
  function renderAll() {
    applyStaticI18n();
    renderLogoGrid();
    renderBrandEditorial();
    renderPricing();
    renderWhy();
    renderFaq();
    renderWizardStep();
  }

  /* =====================================================
     EVENT WIRING
  ===================================================== */
  document.addEventListener("DOMContentLoaded", function () {
    renderAll();

    // Language switcher
    document.querySelectorAll(".lang-btn").forEach(function (btn) {
      btn.addEventListener("click", function () {
        var lang = btn.getAttribute("data-lang-btn");
        if (lang === state.lang) return;
        state.lang = lang;
        renderAll();
      });
    });

    // Mobile nav
    var hamburger = document.getElementById("hamburgerBtn");
    var mobileNav = document.getElementById("mobileNav");
    hamburger.addEventListener("click", function () {
      var open = mobileNav.classList.toggle("open");
      hamburger.classList.toggle("open", open);
      hamburger.setAttribute("aria-expanded", open ? "true" : "false");
    });
    mobileNav.querySelectorAll("a").forEach(function (a) {
      a.addEventListener("click", function () {
        mobileNav.classList.remove("open");
        hamburger.classList.remove("open");
        hamburger.setAttribute("aria-expanded", "false");
      });
    });

    // Service cards -> modal
    document.querySelectorAll(".service-card[data-modal]").forEach(function (card) {
      card.addEventListener("click", function () {
        openServiceModal(card.getAttribute("data-modal"));
      });
    });

    // Portfolio filters
    document.querySelectorAll(".filter-chip").forEach(function (chip) {
      chip.addEventListener("click", function () {
        document.querySelectorAll(".filter-chip").forEach(function (c) { c.classList.remove("active"); });
        chip.classList.add("active");
        state.filter = chip.getAttribute("data-filter");
        document.querySelectorAll("#logoGrid .logo-card").forEach(function (card, i) {
          var item = LOGOS[i];
          card.classList.toggle("hidden", state.filter !== "all" && item.cat !== state.filter);
        });
      });
    });

    // Modal close handlers
    ["serviceModalOverlay", "projectModalOverlay"].forEach(function (id) {
      var overlay = document.getElementById(id);
      overlay.addEventListener("click", function (e) {
        if (e.target === overlay) closeOverlay(id);
      });
    });
    document.getElementById("modalClose").addEventListener("click", function () {
      closeOverlay("serviceModalOverlay");
    });
    document.getElementById("projectModalClose").addEventListener("click", function () {
      closeOverlay("projectModalOverlay");
    });
    document.addEventListener("keydown", function (e) {
      if (e.key === "Escape") {
        closeOverlay("serviceModalOverlay");
        closeOverlay("projectModalOverlay");
      }
    });

    // Wizard nav
    document.getElementById("nextBtn").addEventListener("click", function () {
      if (!validateCurrentStep()) return;
      wizard.stepIndex++;
      renderWizardStep();
      document.getElementById("wizard").scrollIntoView({ behavior: "smooth", block: "start" });
    });
    document.getElementById("backBtn").addEventListener("click", function () {
      wizard.stepIndex = Math.max(0, wizard.stepIndex - 1);
      renderWizardStep();
    });
    document.getElementById("briefForm").addEventListener("submit", handleWizardSubmit);

    initWizard();
    observeReveal();
  });
})();
