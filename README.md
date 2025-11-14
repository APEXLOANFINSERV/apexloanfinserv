## Hi there 👋

<!--
**APEXLOANFINSERV/apexloanfinserv** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->// APEX Loan & Financial Services — Single-file React component
// Uses Tailwind CSS for styling (assumes Tailwind is configured in the project)
// To preview: create a React app (Vite/Create React App) and paste this component into a page.
// Replace placeholder image URLs with actual images (logo and brochure images).

import React from 'react'

export default function ApexWebsite() {
  return (
    <div className="min-h-screen bg-gray-50 text-slate-800">
      {/* Header */}
      <header className="bg-white shadow-sm sticky top-0 z-40">
        <div className="max-w-6xl mx-auto px-6 py-4 flex items-center justify-between">
          <div className="flex items-center gap-4">
            <img src="/logo.png" alt="APEX Logo" className="h-12 w-12 object-contain rounded" onError={(e)=>{e.currentTarget.src='https://via.placeholder.com/80x80?text=APEX'}} />
            <div>
              <h1 className="font-extrabold text-xl text-indigo-700">APEX Loans & Financial Services</h1>
              <p className="text-sm text-slate-500">S-11, Silver Cube Complex, Radhanpur Road, Mehsana</p>
            </div>
          </div>

          <div className="text-right">
            <div className="text-sm text-slate-500">Call / WhatsApp</div>
            <div className="font-semibold text-indigo-700">79845 46752 &nbsp;|&nbsp; 84889 87227</div>
            <div className="text-xs text-slate-400">apexloanfinserv@gmail.com</div>
          </div>
        </div>
      </header>

      {/* Hero */}
      <section className="bg-gradient-to-r from-indigo-50 to-white">
        <div className="max-w-6xl mx-auto px-6 py-12 grid lg:grid-cols-2 gap-8 items-center">
          <div>
            <h2 className="text-3xl lg:text-4xl font-extrabold text-slate-800">One-stop Financial Solutions for Individuals & Businesses</h2>
            <p className="mt-4 text-slate-600 leading-relaxed">Home loans, Business loans, Education loans, Balance Transfer, SIP investment guidance, Health & Vehicle insurance — backed by 33+ years of banking experience and partnerships with 80+ banks and NBFCs.</p>

            <div className="mt-6 flex gap-3">
              <a href="#contact" className="inline-flex items-center px-4 py-2 bg-indigo-600 text-white rounded shadow hover:bg-indigo-700">Get a Free Consultation</a>
              <a href="#services" className="inline-flex items-center px-4 py-2 border border-indigo-600 text-indigo-600 rounded hover:bg-indigo-50">View Services</a>
            </div>

            <ul className="mt-6 grid grid-cols-1 sm:grid-cols-2 gap-2 text-sm text-slate-700">
              <li>• Experienced ex-bank manager team</li>
              <li>• Fast documentation & approval support</li>
              <li>• Lowest possible interest rates</li>
              <li>• End-to-end loan & insurance help</li>
            </ul>
          </div>

          <div className="flex justify-center lg:justify-end">
            <div className="w-full max-w-sm">
              <img src="/brochure-main.jpg" alt="APEX Brochure" className="rounded shadow" onError={(e)=>{e.currentTarget.src='https://via.placeholder.com/420x300?text=Brochure'}} />
              <p className="text-xs text-slate-400 mt-2">Brochure: quick overview of services. Replace with high-res brochure images.</p>
            </div>
          </div>
        </div>
      </section>

      {/* Services */}
      <section id="services" className="max-w-6xl mx-auto px-6 py-12">
        <h3 className="text-2xl font-bold text-slate-800">Our Services</h3>
        <p className="text-slate-600 mt-2">Comprehensive finance products tailored to your needs.</p>

        <div className="mt-6 grid gap-4 grid-cols-1 sm:grid-cols-2 lg:grid-cols-3">
          {[
            {title:'Housing Loan', desc:'Home loan guidance, best rates, quick sanction.'},
            {title:'Balance Transfer (BT)', desc:'Shift to lower interest rates and save.'},
            {title:'Education Loan', desc:'Domestic & international study loan support.'},
            {title:'Business Loan / MSME', desc:'Working capital, project funding & MSME schemes.'},
            {title:'Car & Personal Loan', desc:'Fast approvals, simple documentation.'},
            {title:'SIP Investment Planning', desc:'Systematic investment plans for wealth creation.'},
            {title:'Health & Life Insurance', desc:'Policies from top insurers with claim support.'},
            {title:'Vehicle Insurance', desc:'Two & four wheeler insurance & renewals.'},
            {title:'Project Loan', desc:'Funding for small & medium projects.'}
          ].map((s)=> (
            <div key={s.title} className="p-4 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold text-indigo-700">{s.title}</h4>
              <p className="text-sm text-slate-600 mt-1">{s.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* Why choose us */}
      <section className="bg-indigo-600 text-white">
        <div className="max-w-6xl mx-auto px-6 py-12 grid md:grid-cols-3 gap-8">
          <div>
            <h4 className="font-bold text-lg">33+ Years Banking Experience</h4>
            <p className="mt-2 text-sm">Expert team led by ex-bank managers with deep knowledge of loan processes and documentation.</p>
          </div>
          <div>
            <h4 className="font-bold text-lg">80+ Bank & NBFC Partners</h4>
            <p className="mt-2 text-sm">Strong partnerships to secure the best rates, faster approvals and wider product access.</p>
          </div>
          <div>
            <h4 className="font-bold text-lg">Transparent & Personalized Service</h4>
            <p className="mt-2 text-sm">Tailored advice, clear terms, and end-to-end support from application to disbursal.</p>
          </div>
        </div>
      </section>

      {/* Partners grid (logos) */}
      <section className="max-w-6xl mx-auto px-6 py-12">
        <h3 className="text-xl font-bold">Selected Bank & Insurance Partners</h3>
        <div className="mt-6 grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-6 gap-4 items-center">
          {/* Replace src values with actual partner logos */}
          {Array.from({length:12}).map((_,i)=> (
            <div key={i} className="p-4 bg-white rounded shadow flex items-center justify-center">
              <img src={`https://via.placeholder.com/120x40?text=Bank+${i+1}`} alt={`partner-${i}`} className="max-h-10 object-contain" />
            </div>
          ))}
        </div>
      </section>

      {/* SIP / Investment feature */}
      <section className="bg-gradient-to-r from-green-50 to-white">
        <div className="max-w-6xl mx-auto px-6 py-10 grid md:grid-cols-2 gap-6 items-center">
          <div>
            <h3 className="text-2xl font-bold text-slate-800">SIP Investment Planning</h3>
            <p className="mt-3 text-slate-600">Systematic Investment Plans (SIP) to build long-term wealth. We help you choose suitable funds and create an investment plan aligned with your goals.</p>
            <ul className="mt-3 text-sm text-slate-700 list-disc list-inside">
              <li>Goal-based planning</li>
              <li>Regular review & rebalancing</li>
              <li>Comparison with home loan EMIs for informed decisions</li>
            </ul>
          </div>
          <div>
            <img src="/sip-illustration.jpg" alt="SIP" className="rounded shadow" onError={(e)=>{e.currentTarget.src='https://via.placeholder.com/420x260?text=SIP+Plan'}} />
          </div>
        </div>
      </section>

      {/* Contact */}
      <section id="contact" className="max-w-6xl mx-auto px-6 py-10">
        <div className="grid md:grid-cols-2 gap-8 bg-white rounded-lg p-6 shadow">
          <div>
            <h3 className="text-2xl font-bold">Get in touch</h3>
            <p className="text-slate-600 mt-2">For loan enquiries, consultations or document help, call or WhatsApp us. We provide door-step assistance and quick loan processing support.</p>

            <div className="mt-4">
              <p className="text-sm text-slate-500">Address</p>
              <p className="font-semibold">S-11, Silver Cube Complex, Radhanpur Road, Mehsana</p>

              <p className="mt-3 text-sm text-slate-500">Phone</p>
              <p className="font-semibold">79845 46752, 84889 87227</p>

              <p className="mt-3 text-sm text-slate-500">Email</p>
              <p className="font-semibold">apexloanfinserv@gmail.com</p>
            </div>

            <div className="mt-6 flex gap-3">
              <a href="tel:7984546752" className="inline-block px-4 py-2 bg-indigo-600 text-white rounded">Call Now</a>
              <a href="mailto:apexloanfinserv@gmail.com" className="inline-block px-4 py-2 border border-indigo-600 text-indigo-600 rounded">Email Us</a>
            </div>

            <p className="mt-4 text-xs text-slate-400">Office timings: Mon–Sat 10:00–6:00 (or change as needed)</p>
          </div>

          <div>
            <form action="mailto:apexloanfinserv@gmail.com" method="post" encType="text/plain" className="space-y-3">
              <div>
                <label className="text-sm text-slate-600">Full name</label>
                <input name="name" className="mt-1 w-full border rounded px-3 py-2" required />
              </div>
              <div>
                <label className="text-sm text-slate-600">Phone</label>
                <input name="phone" className="mt-1 w-full border rounded px-3 py-2" required />
              </div>
              <div>
                <label className="text-sm text-slate-600">Service interested</label>
                <select name="service" className="mt-1 w-full border rounded px-3 py-2">
                  <option>Housing Loan</option>
                  <option>Balance Transfer</option>
                  <option>Education Loan</option>
                  <option>Business Loan</option>
                  <option>SIP Investment</option>
                  <option>Insurance</option>
                </select>
              </div>
              <div>
                <label className="text-sm text-slate-600">Message</label>
                <textarea name="message" rows={4} className="mt-1 w-full border rounded px-3 py-2" />
              </div>
              <div>
                <button type="submit" className="inline-block px-4 py-2 bg-green-600 text-white rounded">Send Inquiry</button>
              </div>
            </form>

            <p className="mt-4 text-xs text-slate-400">Alternatively, send WhatsApp message to our number for quick support.</p>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-slate-900 text-white">
        <div className="max-w-6xl mx-auto px-6 py-6 flex flex-col md:flex-row items-center justify-between gap-4">
          <div className="text-sm">© {new Date().getFullYear()} APEX Loans & Financial Services — All rights reserved.</div>
          <div className="text-sm">Contact: 79845 46752
