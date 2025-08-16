# BlendCSS Build Size Checker

# Quick commands to check your CSS build sizes

## Basic PowerShell Commands:

### Check all CSS files:

```powershell
ls css\*.css
```

### Detailed size in KB:

```powershell
Get-ChildItem css\*.css | Select-Object Name, @{Name="Size (KB)";Expression={[math]::Round($_.Length/1KB,2)}}
```

### Compare dev vs production:

```powershell
$dev = (Get-ChildItem css\blend.css).Length
$prod = (Get-ChildItem css\blend.min.css).Length
Write-Host "Dev: $([math]::Round($dev/1KB,2)) KB"
Write-Host "Prod: $([math]::Round($prod/1KB,2)) KB"
Write-Host "Compression: $([math]::Round((1-$prod/$dev)*100,1))%"
```

## NPM Scripts for Building:

### Development build (expanded):

```bash
npm run build
```

### Production build (minified):

```bash
npm run build:prod
```

### Watch mode (auto-rebuild):

```bash
npm run dev
```

## Current Sizes (Week 1):

- **Development**: ~34 KB (34,601 bytes)
- **Production**: ~24 KB (23,820 bytes)
- **Compression**: ~31% reduction
- **Gzipped estimate**: ~6-8 KB (typical for CSS)

## Size Targets by Week:

- Week 1: ✅ ~34 KB (Foundation + Typography + Classless)
- Week 2: ~45-55 KB (+ Utilities)
- Week 3: ~60-70 KB (+ Components)
- Week 4: ~75-85 KB (+ Advanced Features)
- Final: Target <100 KB unminified, <70 KB minified

## Framework Size Comparison:

- **Bootstrap 5**: ~160 KB (minified)
- **Tailwind CSS**: ~300+ KB (full build)
- **Bulma**: ~180 KB
- **BlendCSS**: Target ~70 KB (hybrid approach)

## Optimization Tips:

1. Use production build for deployment
2. Enable gzip compression on server
3. Consider tree-shaking unused utilities in Week 2+
4. Monitor size growth each week
