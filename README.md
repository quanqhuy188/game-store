### Convention code

- [Commit-lint](https://github.com/conventional-changelog/commitlint)
- [Naming](https://github.com/kettanaito/naming-cheatsheet)
- [Clean code](https://github.com/ryanmcdermott/clean-code-javascript#table-of-contents)
- [react-philosophies](https://github.com/mithi/react-philosophies)

#### Một số điểm cần lưu ý
- Sử dụng yarn để quản lý node package.
- Khi commit cần commit, đặt tên biến, và React cần tuân thủ theo convention ở trên. (Cần đọc kĩ và ghi nhớ).
- Cần cài đặt Format file bằng prettier.
- Khi cài thư viện, nếu cần cài @type thì cài vào devDependencies. ví dụ:
    - `yarn add -D @types/lodash.isequal`
- Đặt tên thư mục theo kiểu kebab-case, ví dụ:
    - `src/components/home`
    - `src/components/home-section`
- Mỗi thư mục có một file index.ts để xuất file, ví dụ:
    - `src/components/home/index.ts`
- Nếu file là một React Component, đặt tên file giống tên Component. Kiểu PascalCase, ví dụ:
    - `src/components/home/Home.tsx`
    - `src/components/home/components/HomeCardExample.tsx`


##### Lưu ý với MUI
- Tất cả các config về theme như: màu sắc, fontSize, fontFamily, ... đều config trong thư mục `src/lib/theme`.
- Không dùng inline style kiểu này: `sx={{ color: '#fffff' }}`.
  - Thay vào đó nên dùng `sx={{color: theme => theme.palette.common.white}}` hoặc `sx={{color: common.white}}`.
- [Customization MUI component](https://mui.com/material-ui/customization/how-to-customize/)
- Chỉ cài thêm lib khi thực sự cần thiết.
- [Khi nào thì sử dụng sx hay styled](https://mui.com/system/basics/#the-sx-prop)
