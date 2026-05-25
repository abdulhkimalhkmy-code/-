export default function BasmatDesignApp() { const products = [ { title: 'طباعة على كوب عادي', price: '1000 ريال' }, { title: 'طباعة على كوب سحري', price: '1500 ريال' }, { title: 'طباعة على صحن', price: '1200 ريال' }, { title: 'طباعة على تيشيرت', price: '1000 ريال' }, { title: 'طباعة على ميدالية', price: '250 ريال' }, { title: 'طباعة على غلاف جوال', price: '2500 ريال' }, ];

return ( <div className="min-h-screen bg-slate-950 text-white" dir="rtl"> <header className="bg-slate-900 border-b border-yellow-500 p-6 flex flex-col items-center"> <img
src="https://placehold.co/200x120/png"
alt="Basmat Design"
className="rounded-2xl mb-4"
/> <h1 className="text-4xl font-bold text-yellow-400 mb-2"> بصمة ديزاين </h1> <p className="text-lg text-slate-300"> للتصوير والدعاية والإعلان </p> </header>

<section className="p-6">
    <div className="bg-gradient-to-l from-yellow-500 to-orange-500 rounded-3xl p-8 shadow-2xl text-center">
      <h2 className="text-3xl font-bold mb-4 text-slate-900">
        أهلاً بك في متجر بصمة ديزاين
      </h2>
      <p className="text-slate-900 text-lg">
        اطلب خدمات الطباعة والتصميم والتصوير بسهولة
      </p>
    </div>
  </section>

  <section className="p-6 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
    {products.map((item, index) => (
      <div
        key={index}
        className="bg-slate-900 rounded-3xl shadow-xl overflow-hidden border border-slate-700"
      >
        <img
          src="https://placehold.co/600x400/png"
          alt={item.title}
          className="w-full h-52 object-cover"
        />

        <div className="p-5">
          <h3 className="text-2xl font-bold mb-3 text-yellow-400">
            {item.title}
          </h3>

          <p className="text-xl text-white mb-5">
            {item.price}
          </p>

          <a
            href="https://wa.me/967780994036"
            target="_blank"
            className="block text-center bg-green-500 hover:bg-green-600 transition rounded-2xl py-3 text-lg font-bold"
          >
            اطلب الآن عبر واتساب
          </a>
        </div>
      </div>
    ))}
  </section>

  <footer className="bg-slate-900 border-t border-yellow-500 p-6 text-center mt-10">
    <p className="text-yellow-400 text-xl font-bold mb-2">
      بصمة ديزاين للتصوير والدعاية والإعلان
    </p>
    <p className="text-slate-300">
      واتساب: +967 780 994 036
    </p>
  </footer>
</div>

); }# -
بصمة ديزاين للتصوير والدعاية والإعلان 
