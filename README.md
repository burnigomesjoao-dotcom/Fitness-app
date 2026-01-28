package.json
{
  "name": "fitness-app",
  "private": true,
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start"
  },
  "dependencies": {
    "next": "14.1.0",
    "react": "18.2.0",
    "react-dom": "18.2.0"
  }
}
app/page.js
export default function Home() {
  return (
    <main style={{
      minHeight: '100vh',
      display: 'flex',
      justifyContent: 'center',
      alignItems: 'center',
      flexDirection: 'column',
      fontFamily: 'Arial'
    }}>
      <h1>🏋️ Fitness App</h1>
      <p>Criado 100% pelo iPhone 🚀</p>
    </main>
  )
}
app/layout.js
export const metadata = {
  title: 'Fitness App',
  description: 'Aplicativo fitness',
}

export default function RootLayout({ children }) {
  return (
    <html lang="pt-BR">
      <body>{children}</body>
    </html>
  )
}