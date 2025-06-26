# Katkıda Bulunma Rehberi

Nova SEO Frontend Dashboard projesine katkıda bulunmak istediğiniz için teşekkür ederiz! 🚀

## 🤝 Nasıl Katkıda Bulunabilirsiniz

### 1. Geliştirme Ortamını Kurma

```bash
# Repository'yi fork edin ve klonlayın
git clone https://github.com/YOUR_USERNAME/NovaSEO-Frontend-Dashboard-Updated.git
cd NovaSEO-Frontend-Dashboard-Updated

# Bağımlılıkları yükleyin
pnpm install

# Geliştirme sunucusunu başlatın
pnpm dev
```

### 2. Branch Oluşturma

```bash
# Ana daldan yeni bir branch oluşturun
git checkout -b feature/your-feature-name

# Örnek branch isimleri:
# feature/add-new-seo-tool
# fix/mobile-responsiveness
# docs/update-readme
```

### 3. Kod Yazma Standartları

#### TypeScript
- Tüm yeni kod TypeScript ile yazılmalıdır
- Strict mode kullanın
- Type definitions için interface kullanın

#### React Bileşenleri
- Functional components kullanın
- Hooks'ları tercih edin
- Props için TypeScript interfaces tanımlayın

```tsx
interface ComponentProps {
  title: string
  description?: string
  onAction: () => void
}

const MyComponent: React.FC<ComponentProps> = ({ title, description, onAction }) => {
  // Component logic
}
```

#### Styling
- Tailwind CSS kullanın
- Shadcn/UI bileşenlerini tercih edin
- Custom CSS'den kaçının

#### Dosya Yapısı
```
components/
├── ui/              # Shadcn/UI bileşenleri
├── pages/           # Sayfa bileşenleri
└── shared/          # Paylaşılan bileşenler

app/
├── dashboard/       # Dashboard sayfaları
└── api/            # API routes

lib/
└── utils.ts        # Utility fonksiyonlar

hooks/
└── use-*.ts        # Custom hooks
```

### 4. Commit Kuralları

Conventional Commits formatını kullanın:

```bash
# Yeni özellik
git commit -m "feat: add keyword tracking dashboard"

# Bug düzeltme
git commit -m "fix: resolve mobile sidebar issue"

# Dokümantasyon
git commit -m "docs: update API documentation"

# Stil değişiklikleri
git commit -m "style: improve button hover effects"

# Refactoring
git commit -m "refactor: optimize search algorithm"
```

### 5. Pull Request Süreci

1. **Fork & Branch**: Repository'yi fork edin ve feature branch oluşturun
2. **Develop**: Değişikliklerinizi yapın
3. **Test**: Kodunuzun çalıştığından emin olun
4. **Commit**: Conventional commit formatında commit'leyin
5. **Push**: Branch'inizi push edin
6. **PR**: Pull Request oluşturun

#### PR Template
```markdown
## 📝 Değişiklik Açıklaması
Kısa bir açıklama...

## 🎯 Değişiklik Türü
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## ✅ Checklist
- [ ] Kod TypeScript kurallarına uygun
- [ ] Responsive tasarım test edildi
- [ ] SEO optimizasyonları kontrol edildi
- [ ] Accessibility kurallarına uygun
```

### 6. UI/UX Kuralları

#### Responsive Design
- Mobile-first yaklaşım
- Breakpoints: 640px (sm), 768px (md), 1024px (lg), 1280px (xl)
- Touch-friendly butonlar (minimum 44px)

#### Accessibility
- ARIA labels kullanın
- Keyboard navigation desteği
- Color contrast kurallarına uyun
- Screen reader desteği

#### Performance
- Lazy loading kullanın
- Image optimization
- Code splitting
- Minimal bundle size

### 7. SEO Kuralları

- Semantic HTML kullanın
- Meta tags ekleyin
- Structured data desteği
- Fast loading times
- Clean URLs

### 8. Test Etme

```bash
# Lint kontrolü
pnpm lint

# Build test
pnpm build

# Type check
npx tsc --noEmit
```

### 9. Sorun Bildirme

Sorun bildirirken şunları dahil edin:
- Sorunun açıklaması
- Tekrarlama adımları
- Beklenen davranış
- Ekran görüntüleri
- Tarayıcı/OS bilgileri

### 10. İletişim

- GitHub Issues: Teknik sorular ve bug raporları
- Discussions: Genel tartışmalar ve öneriler

## 🎨 Design System

### Renkler
- Primary: Blue (SEO focus)
- Secondary: Gray scales
- Success: Green
- Warning: Orange
- Error: Red

### Typography
- Font: Inter
- Sizes: text-sm, text-base, text-lg, text-xl, text-2xl

### Spacing
- Margin/Padding: 4px grid system
- Gap: space-2, space-4, space-6, space-8

## 📚 Faydalı Linkler

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [Shadcn/UI](https://ui.shadcn.com/)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)

## 🏆 Katkıda Bulunanlar

Tüm katkıda bulunanlara teşekkür ederiz! Sizin katkılarınız bu projeyi daha iyi hale getiriyor.

---

**Unutmayın:** Her katkı değerlidir, küçük düzeltmelerden büyük özelliklere kadar her şey memnuniyetle karşılanır! 🙏