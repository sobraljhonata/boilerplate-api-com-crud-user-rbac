
# INSTRUÇÕES DE USO

```bash
sudo apt-get update -y && sudo apt-get upgrade -y && \

sudo apt update -y && sudo apt install git -y && \

git config --global core.editor 'code --wait' && \
git config --global init.defaultBranch main && \
git config --global --edit && \

cd ~ && \

mkdir -p ~/Projetos && \

cd ~/Projetos && \

git clone https://github.com/sobraljhonata/script-python-senac.git && \

git clone https://github.com/sobraljhonata/boilerplate-api-com-crud-user-rbac.git && \

python3 ~/Projetos/script-python-senac/gerador-api-node-express/main.py && \

mkdir -p ~/Projetos/<nome_do_projeto> && \

cd ~/Projetos/<nome_do_projeto> && \

cp ~/Projetos/boilerplate-api-com-crud-user-rbac/jest-integration-config.js ~/Projetos/boilerplate-api-com-crud-user-rbac/jest-unit-config.ts ~/Projetos/boilerplate-api-com-crud-user-rbac/jest.config.ts ~/Projetos/boilerplate-api-com-crud-user-rbac/nodemon.json ~/Projetos/boilerplate-api-com-crud-user-rbac/tsconfig.json ~/Projetos/boilerplate-api-com-crud-user-rbac/.env-exemplo ~/Projetos/boilerplate-api-com-crud-user-rbac/.gitignore ~/Projetos/boilerplate-api-com-crud-user-rbac/tsconfig.build.json ~/Projetos/boilerplate-api-com-crud-user-rbac/tsconfig.spec.json ~/Projetos/boilerplate-api-com-crud-user-rbac/yarn.lock ~/Projetos/<nome_do_projeto> && \

mkdir -p ~/Projetos/<nome_do_projeto>/src/core ~/Projetos/<nome_do_projeto>/src/modules ~/Projetos/<nome_do_projeto>/test/unit/modules && \

cp -r ~/Projetos/boilerplate-api-com-crud-user-rbac/src/core ~/Projetos/<nome_do_projeto>/src && \

cp -r ~/Projetos/boilerplate-api-com-crud-user-rbac/src/modules/auth ~/Projetos/boilerplate-api-com-crud-user-rbac/src/modules/users ~/Projetos/<nome_do_projeto>/src/modules && \

cp ~/Projetos/boilerplate-api-com-crud-user-rbac/src/server.ts ~/Projetos/<nome_do_projeto>/src && \

cp ~/Projetos/boilerplate-api-com-crud-user-rbac/.env-exemplo ~/Projetos/<nome_do_projeto>/.env && \

cp -r ~/Projetos/boilerplate-api-com-crud-user-rbac/test/factories ~/Projetos/boilerplate-api-com-crud-user-rbac/test/helpers ~/Projetos/boilerplate-api-com-crud-user-rbac/test/integration ~/Projetos/<nome_do_projeto>/test && \

cp -r ~/Projetos/boilerplate-api-com-crud-user-rbac/test/unit/adapters ~/Projetos/boilerplate-api-com-crud-user-rbac/test/unit/core ~/Projetos/boilerplate-api-com-crud-user-rbac/test/unit/middlewares ~/Projetos/<nome_do_projeto>/test/unit && \

cp -r ~/Projetos/boilerplate-api-com-crud-user-rbac/test/unit/modules/auth ~/Projetos/boilerplate-api-com-crud-user-rbac/test/unit/modules/users ~/Projetos/<nome_do_projeto>/test/unit/modules && \

yarn init -y && \

npm pkg set scripts.dev="nodemon" && \
npm pkg set scripts.build:clean="npm run clear:packages && npm run build" && \
npm pkg set scripts.clear:packages="rimraf package-lock.json && rimraf dist && rimraf tsconfig.tsbuildinfo && rimraf node_modules &&npm install" && \
npm pkg set scripts.build="NODE_ENV=production tsc -p tsconfig.json && tsc-alias -p tsconfig.json && npm run copy:swagger" && \
npm pkg set scripts.start="node dist/server.js" && \
npm pkg set scripts.start:debug="node --inspect dist/server.js" && \
npm pkg set scripts.typecheck="tsc -p tsconfig.json --noEmit" && \
npm pkg set scripts.copy:swagger="copyfiles -u 2 \"src/docs/**/*\" dist/docs" && \
npm pkg set scripts.test="NODE_ENV=test jest --passWithNoTests --silent --noStackTrace --runInBand" && \
npm pkg set scripts.test:verbose="NODE_ENV=test jest --passWithNoTests --runInBand" && \
npm pkg set scripts.test:clear="npx jest --clearCache" && \
npm pkg set scripts.test:unit="npm test -- --watchAll -c jest-unit-config.ts" && \
npm pkg set scripts.test:integration="npm test -- --watchAll -c jest-integration-config.js" && \
npm pkg set scripts.test:staged="npm test -- --findRelatedTests" && \
npm pkg set scripts.test:ci="npm test -- --coverage"

yarn add -D @types/bcrypt@^5.0.2 @types/dotenv@^8.2.3 @types/express@^5.0.2 @types/jest@^29.5.13 @types/jsonwebtoken@^9.0.9 @types/node@^22.15.21 @types/supertest@^6.0.3 @types/swagger-jsdoc@^6.0.4 @types/swagger-ui-express@^4.1.8 @types/yamljs@^0.2.34 copyfiles@^2.4.1 jest@^29.7.0 nodemon@^3.1.10 rimraf@^6.0.1 sqlite3@^5.1.7 supertest@^7.1.4 ts-jest@^29.2.5 ts-node@^10.9.2 tsc-alias@^1.8.16 tsconfig-paths@^4.2.0 typescript@^5.8.3 && \

yarn add bcrypt@^6.0.0 dotenv@^16.5.0 express@^5.1.0 fast-glob@^3.3.3 jsonwebtoken@^9.0.2 module-alias@^2.2.3 mysql2@^3.14.1 sequelize@^6.37.7 swagger-jsdoc@^6.2.8 swagger-ui-express@^5.0.1 yamljs@^0.3.0 zod@^4.1.12 && \

npm pkg set _moduleAliases.@="dist" && \

sudo rm -rf ~/Projetos/boilerplate-api-com-crud-user-rbac ~/Projetos/script-python-senac && \

cd ~/Projetos/<nome_do_projeto> && \
git init && \
git add --all && \
git commit -am "initial"
```
