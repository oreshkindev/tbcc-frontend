<template>
    <main>
        <section class="c">
            <main-heading :message="$t('post[0][0]')" />

            <div class="container row">
                <div class="col-sm-12 col-md-6">
                    <p>
                        {{ $t('post[0][1]') }}
                    </p>
                    <p>
                        {{ $t('post[0][2]') }}
                    </p>
                    <p>
                        {{ $t('post[0][3]') }}
                    </p>
                    <p>
                        {{ $t('post[0][4]') }}
                    </p>
                    <blockquote>
                        {{ $t('post[0][5]') }}
                    </blockquote>
                    <h4>
                        {{ $t('post[0][6]') }}
                    </h4>
                    <p>
                        {{ $t('post[0][7]') }}
                    </p>
                    <h4>{{ $t('post[0][8]') }}</h4>
                    <p>
                        {{ $t('post[0][9]') }}
                    </p>
                    <h4>{{ $t('post[0][10]') }}</h4>
                    <ul>
                        <li>
                            {{ $t('post[0][11]') }}
                        </li>
                    </ul>
                    <h4>
                        {{ $t('post[0][12]') }}
                    </h4>
                    <ul>
                        <li>
                            {{ $t('post[0][13]') }}
                        </li>
                    </ul>
                    <h4>{{ $t('post[0][14]') }}</h4>
                    <ul>
                        <li>
                            {{ $t('post[0][15]') }}
                        </li>
                    </ul>
                    <h4>{{ $t('post[0][16]') }}</h4>
                    <p>
                        {{ $t('post[0][17]') }}
                    </p>
                </div>

                <div class="col-sm-12 col-md-6">
                    <h4>{{ $t('post[0][18]') }}</h4>
                    <p>
                        {{ $t('post[0][19]') }}
                    </p>
                    <p>
                        {{ $t('post[0][20]') }}
                    </p>
                    <h4>{{ $t('post[0][21]') }}</h4>
                    <p>
                        {{ $t('post[0][22]') }}
                    </p>
                    <p>
                        {{ $t('post[0][23]') }}
                    </p>
                    <h4>
                        {{ $t('post[0][24]') }}
                    </h4>
                    <p>
                        {{ $t('post[0][25]') }}
                    </p>
                    <p>
                        {{ $t('post[0][26]') }}
                    </p>
                    <ul>
                        <li>
                            {{ $t('post[0][27]') }}
                        </li>
                        <li>
                            {{ $t('post[0][28]') }}
                        </li>
                    </ul>
                    <p>
                        {{ $t('post[0][29]') }}
                    </p>
                    <h4>{{ $t('post[0][30]') }}</h4>
                    <p>
                        {{ $t('post[0][31]') }}
                    </p>
                </div>

                <div class="col-sm-12 col-md-6">
                    <figure>
                        <img :src="require('@/assets/blank.svg')" alt="" />
                    </figure>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
main {
    section {
        .container {
            margin: 1em auto;
            max-width: 1480px;
        }
    }

    p {
        padding: 0 2em 1em;
    }
    ul {
        list-style: none;
        margin: 0;
        padding: 0 2em;

        li {
            margin: 1em 0;
            position: relative;

            &::before {
                color: var(--theme-color);
                content: '';
                left: -25px;
                position: absolute;
                top: 11px;
                border: 2px solid;
                width: 18px;
            }
        }
    }
}

.heading {
    justify-content: start !important;
    margin: 2em auto 6em !important;

    @media only screen and (max-width: 767.98px) {
        margin: 2em auto !important;
    }
}

.c {
    &::before {
        content: '';
        background: var(--theme-color);
        mask-image: url('~@/assets/c.svg');
        mask-repeat: no-repeat;
        mask-size: 780px;
        mask-position: right top;
        position: absolute;
        width: 100%;
        height: 100%;
    }
}

figure {
    margin: 0 2em;
    img {
        width: 100%;
        height: 100%;
        vertical-align: middle;
    }
}

blockquote {
    background: var(--theme-color);
    margin: 2em 2em 1.6em;
    padding: 2em;
    position: relative;
    z-index: 0;

    &::before {
        content: '”';
        font-size: 12em;
        line-height: 0;
        position: absolute;
        top: -45px;
        left: 0;
        transform: rotate(180deg);
        z-index: -1;
    }
}

h1,
h2,
h3,
h4 {
    font-weight: 300;
    text-transform: uppercase;
}

h1 {
    font-size: 36px;
}

h2 {
    font-size: 28px;
}

h3 {
    font-size: 24px;
}

h4 {
    color: var(--theme-color);
    font-size: 18px;
    margin: 0 2em 1em;
}

span {
    color: var(--theme-color);
    text-transform: uppercase;
}
</style>
